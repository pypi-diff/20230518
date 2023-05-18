# Comparing `tmp/netbox-routing-0.0.1.tar.gz` & `tmp/netbox-routing-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/netbox-routing-0.0.1.tar", last modified: Mon Apr  4 22:13:55 2022, max compression
+gzip compressed data, was "dist/netbox-routing-0.0.2.tar", last modified: Thu May 18 03:11:22 2023, max compression
```

## Comparing `netbox-routing-0.0.1.tar` & `netbox-routing-0.0.2.tar`

### file list

```diff
@@ -1,74 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/api/nested_serializers/
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/api/nested_serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1351 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/api/nested_serializers/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/api/nested_serializers/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/api/serializers/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/api/serializers/static.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/api/views/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/api/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/api/views/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/api/views/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/choices/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/choices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/choices/bgp.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/choices/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/constants/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/constants/bgp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/fields/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/fields/ip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/filtersets/
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/filtersets/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/filtersets/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/forms/
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/forms/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/forms/filtersets/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/forms/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/forms/filtersets/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/forms/filtersets/static.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/forms/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/forms/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/models/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8382 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/models/bgp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/models/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/models/static.py
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/tables/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/tables/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/tables/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/templates/netbox_routing/
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/templates/netbox_routing/staticroute.html
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing/views/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2746 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/views/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/netbox_routing/views/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/netbox_routing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-04 22:13:55.000000 netbox-routing-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-04-04 22:13:47.000000 netbox-routing-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/api/nested_serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/api/nested_serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/api/nested_serializers/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/api/nested_serializers/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/api/serializers/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/api/serializers/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/api/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/api/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/api/views/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/api/views/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/choices/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/choices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/choices/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/choices/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/constants/bgp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/fields/ip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/filtersets/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/filtersets/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/forms/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/forms/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/forms/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/forms/filtersets/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/forms/filtersets/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/forms/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/forms/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/models/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/models/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/models/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/models/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/tables/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/tables/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/templates/netbox_routing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/templates/netbox_routing/staticroute.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/views/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/netbox_routing/views/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/netbox_routing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 03:11:22.000000 netbox-routing-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-18 03:11:16.000000 netbox-routing-0.0.2/setup.py
```

### Comparing `netbox-routing-0.0.1/LICENSE` & `netbox-routing-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/PKG-INFO` & `netbox-routing-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: netbox-routing
-Version: 0.0.1
+Version: 0.0.2
 Summary: NetBox Routing
 Home-page: https://github.com/dansheps/netbox-routing/
 Download-URL: https://pypi.org/project/netbox-routing/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
 License: All rights reserved
 Keywords: netbox,netbox-plugin
-Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 Plugin for documentation of routing configuration and objects
-
```

### Comparing `netbox-routing-0.0.1/README.md` & `netbox-routing-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 A plugin for tracking all kinds of routing information
 
 ## Features
 
 ### Current features
 
 * Static routing
+
+### Under development
+
 * Dynamic routing
   * BGP
     * Templates/Group inheritance
   * OSPF
 
 ### Roadmapped
```

### Comparing `netbox-routing-0.0.1/netbox_routing/__init__.py` & `netbox-routing-0.0.2/netbox_routing/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from extras.plugins import PluginConfig
+from importlib.metadata import metadata
 
-try:
-    from importlib.metadata import metadata
-except ModuleNotFoundError:
-    from importlib_metadata import metadata
 
 plugin = metadata('netbox_routing')
 
 
 class NetboxRouting(PluginConfig):
     name = plugin.get('Name').replace('-', '_')
     verbose_name = plugin.get('Summary')
```

### Comparing `netbox-routing-0.0.1/netbox_routing/api/nested_serializers/objects.py` & `netbox-routing-0.0.2/netbox_routing/api/nested_serializers/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from rest_framework import serializers
 
-from netbox.api import WritableNestedSerializer
+from netbox.api.serializers import WritableNestedSerializer
 from netbox_routing.models import PrefixList, PrefixListEntry, RouteMap, RouteMapEntry
 
 
 __all__ = (
     'NestedStaticRouteSerializer'
 )
```

### Comparing `netbox-routing-0.0.1/netbox_routing/api/serializers/objects.py` & `netbox-routing-0.0.2/netbox_routing/api/serializers/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/api/serializers/static.py` & `netbox-routing-0.0.2/netbox_routing/api/serializers/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/api/views/objects.py` & `netbox-routing-0.0.2/netbox_routing/api/views/objects.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from netbox.api.viewsets import ModelViewSet
+from netbox.api.viewsets import NetBoxModelViewSet
 from netbox_routing.api.serializers import PrefixListSerializer, PrefixListEntrySerializer, RouteMapSerializer, \
     RouteMapEntrySerializer
 from netbox_routing.models import PrefixList, PrefixListEntry, RouteMap, RouteMapEntry
 
 
-class PrefixListViewSet(ModelViewSet):
+class PrefixListViewSet(NetBoxModelViewSet):
     queryset = PrefixList.objects.all()
     serializer_class = PrefixListSerializer
 
 
-class PrefixListEntryViewSet(ModelViewSet):
+class PrefixListEntryViewSet(NetBoxModelViewSet):
     queryset = PrefixListEntry.objects.all()
     serializer_class = PrefixListEntrySerializer
 
 
-class RouteMapViewSet(ModelViewSet):
+class RouteMapViewSet(NetBoxModelViewSet):
     queryset = RouteMap.objects.all()
     serializer_class = RouteMapSerializer
 
 
-class RouteMapEntryViewSet(ModelViewSet):
+class RouteMapEntryViewSet(NetBoxModelViewSet):
     queryset = RouteMapEntry.objects.all()
     serializer_class = RouteMapEntrySerializer
```

### Comparing `netbox-routing-0.0.1/netbox_routing/choices/bgp.py` & `netbox-routing-0.0.2/netbox_routing/choices/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/constants/bgp.py` & `netbox-routing-0.0.2/netbox_routing/constants/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/fields/ip.py` & `netbox-routing-0.0.2/netbox_routing/fields/ip.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/filtersets/objects.py` & `netbox-routing-0.0.2/netbox_routing/filtersets/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/filtersets/static.py` & `netbox-routing-0.0.2/netbox_routing/filtersets/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/forms/objects.py` & `netbox-routing-0.0.2/netbox_routing/forms/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/forms/static.py` & `netbox-routing-0.0.2/netbox_routing/forms/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/models/bgp.py` & `netbox-routing-0.0.2/netbox_routing/models/bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/models/objects.py` & `netbox-routing-0.0.2/netbox_routing/models/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/models/static.py` & `netbox-routing-0.0.2/netbox_routing/models/static.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/navigation.py` & `netbox-routing-0.0.2/netbox_routing/navigation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-from extras.plugins import PluginMenuButton, PluginMenuItem
+from extras.plugins import PluginMenuButton, PluginMenuItem, PluginMenu
 from utilities.choices import ButtonColorChoices
 
-menu_items = (
-    PluginMenuItem(
-        link='plugins:netbox_routing:staticroute_list',
-        link_text='Static Route',
-        buttons=(
-            PluginMenuButton('plugins:netbox_routing:staticroute_add', 'Add', 'mdi mdi-plus', ButtonColorChoices.GREEN),
-            PluginMenuButton('plugins:netbox_routing:staticroute_import', 'Import', 'mdi mdi-upload', ButtonColorChoices.CYAN),
-        )
-    ),
-    PluginMenuItem(
-        link='plugins:netbox_routing:prefixlist_list',
-        link_text='Prefix Lists',
-        buttons=(
-            PluginMenuButton('plugins:netbox_routing:prefixlist_add', 'Add', 'mdi mdi-plus', ButtonColorChoices.GREEN),
-            PluginMenuButton('plugins:netbox_routing:prefixlist_import', 'Import', 'mdi mdi-upload', ButtonColorChoices.CYAN),
-        )
-    ),
-    PluginMenuItem(
-        link='plugins:netbox_routing:routemap_list',
-        link_text='Route Maps',
-        buttons=(
-            PluginMenuButton('plugins:netbox_routing:routemap_add', 'Add', 'mdi mdi-plus', ButtonColorChoices.GREEN),
-            PluginMenuButton('plugins:netbox_routing:routemap_import', 'Import', 'mdi mdi-upload', ButtonColorChoices.CYAN),
-        )
+static = PluginMenuItem(
+    link='plugins:netbox_routing:staticroute_list',
+    link_text='Static Route',
+    buttons=(
+        PluginMenuButton('plugins:netbox_routing:staticroute_add', 'Add', 'mdi mdi-plus', ButtonColorChoices.GREEN),
+        PluginMenuButton('plugins:netbox_routing:staticroute_import', 'Import', 'mdi mdi-upload', ButtonColorChoices.CYAN),
+    )
+)
+prefixlist = PluginMenuItem(
+    link='plugins:netbox_routing:prefixlist_list',
+    link_text='Prefix Lists',
+    buttons=(
+        PluginMenuButton('plugins:netbox_routing:prefixlist_add', 'Add', 'mdi mdi-plus', ButtonColorChoices.GREEN),
+        PluginMenuButton('plugins:netbox_routing:prefixlist_import', 'Import', 'mdi mdi-upload', ButtonColorChoices.CYAN),
+    )
+)
+routemap = PluginMenuItem(
+    link='plugins:netbox_routing:routemap_list',
+    link_text='Route Maps',
+    buttons=(
+        PluginMenuButton('plugins:netbox_routing:routemap_add', 'Add', 'mdi mdi-plus', ButtonColorChoices.GREEN),
+        PluginMenuButton('plugins:netbox_routing:routemap_import', 'Import', 'mdi mdi-upload', ButtonColorChoices.CYAN),
+    )
+)
+
+menu = PluginMenu(
+    label='Netbox Routing',
+    groups=(
+        ('Routing Objects', (prefixlist, routemap )),
+        ('Support Contracts', (static, )),
     ),
-)
+    icon_class='mdi mdi-router'
+)
```

### Comparing `netbox-routing-0.0.1/netbox_routing/tables/objects.py` & `netbox-routing-0.0.2/netbox_routing/tables/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/templates/netbox_routing/staticroute.html` & `netbox-routing-0.0.2/netbox_routing/templates/netbox_routing/staticroute.html`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/urls.py` & `netbox-routing-0.0.2/netbox_routing/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 urlpatterns = [
     path('routes/static/', views.StaticRouteListView.as_view(), name='staticroute_list'),
     path('routes/static/add/', views.StaticRouteEditView.as_view(), name='staticroute_add'),
     path('routes/static/import/', views.StaticRouteListView.as_view(), name='staticroute_import'),
     path('routes/static/<int:pk>/', views.StaticRouteView.as_view(), name='staticroute'),
     path('routes/static/<int:pk>/edit/', views.StaticRouteEditView.as_view(), name='staticroute_edit'),
+    path('routes/static/<int:pk>/devices/', views.StaticRouteDevicesView.as_view(), name='staticroute_devices'),
     path('routes/static/<int:pk>/delete/', views.StaticRouteDeleteView.as_view(), name='staticroute_delete'),
     path('routes/static/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='staticroute_changelog', kwargs={'model': StaticRoute}),
 
     path('prefix-list/', views.PrefixListListView.as_view(), name='prefixlist_list'),
     path('prefix-list/add/', views.PrefixListEditView.as_view(), name='prefixlist_add'),
     path('prefix-list/import/', views.PrefixListListView.as_view(), name='prefixlist_import'),
     path('prefix-list/<int:pk>/', views.PrefixListView.as_view(), name='prefixlist'),
```

### Comparing `netbox-routing-0.0.1/netbox_routing/views/__init__.py` & `netbox-routing-0.0.2/netbox_routing/views/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from .static import StaticRouteListView, StaticRouteEditView, StaticRouteView, StaticRouteDeleteView
+from .static import StaticRouteListView, StaticRouteDevicesView, StaticRouteEditView, StaticRouteView, \
+    StaticRouteDeleteView
 
 from .objects import PrefixListView, PrefixListEditView, PrefixListListView, PrefixListDeleteView, RouteMapListView, \
     RouteMapView, RouteMapEditView, RouteMapDeleteView, PrefixListEntryListView, PrefixListEntryEditView, \
     PrefixListEntryDeleteView, PrefixListEntryView, RouteMapEntryListView, RouteMapEntryView, RouteMapEntryEditView, \
     RouteMapEntryDeleteView
 
 __all__ = (
     'StaticRouteListView',
     'StaticRouteView',
+    'StaticRouteDevicesView',
     'StaticRouteEditView',
     'StaticRouteDeleteView',
 
     'PrefixListListView',
     'PrefixListView',
     'PrefixListEditView',
     'PrefixListDeleteView',
```

### Comparing `netbox-routing-0.0.1/netbox_routing/views/objects.py` & `netbox-routing-0.0.2/netbox_routing/views/objects.py`

 * *Files identical despite different names*

### Comparing `netbox-routing-0.0.1/netbox_routing/views/static.py` & `netbox-routing-0.0.2/netbox_routing/views/static.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,38 @@
+from dcim.filtersets import DeviceFilterSet
 from dcim.models import Device
 from dcim.tables import DeviceTable
-from netbox.views.generic import ObjectListView, ObjectEditView, ObjectView, ObjectDeleteView
+from netbox.views.generic import ObjectListView, ObjectEditView, ObjectView, ObjectDeleteView, ObjectChildrenView
 from netbox_routing.filtersets.static import StaticRouteFilterSet
 from netbox_routing.forms import StaticRouteForm
 from netbox_routing.forms.filtersets.static import StaticRouteFilterSetForm
 from netbox_routing.models import StaticRoute
 from netbox_routing.tables.static import StaticRouteTable
 
 
 __all__ = (
     'StaticRouteListView',
     'StaticRouteView',
+    'StaticRouteDevicesView',
     'StaticRouteEditView',
     'StaticRouteDeleteView',
 )
 
+from utilities.views import register_model_view, ViewTab
 
+
+@register_model_view(StaticRoute, name='list')
 class StaticRouteListView(ObjectListView):
     queryset = StaticRoute.objects.all()
     table = StaticRouteTable
     filterset = StaticRouteFilterSet
     filterset_form = StaticRouteFilterSetForm
 
 
+@register_model_view(StaticRoute)
 class StaticRouteView(ObjectView):
     queryset = StaticRoute.objects.all()
     template_name = 'netbox_routing/staticroute.html'
 
     def get_extra_context(self, request, instance):
         devices = instance.devices.all()
 
@@ -39,14 +45,33 @@
         )
 
         return {
             'devices': devices_table,
         }
 
 
+@register_model_view(StaticRoute, name='assignments')
+class StaticRouteDevicesView(ObjectChildrenView):
+    # template_name = 'dcim//.html'
+    queryset = StaticRoute.objects.all()
+    child_model = Device
+    table = DeviceTable
+    filterset = DeviceFilterSet
+    actions = []
+    tab = ViewTab(
+        label='Assigned Devices',
+        badge=lambda obj: Device.objects.filter(static_routes=obj).count(),
+    )
+
+    def get_children(self, request, parent):
+        return self.child_model.objects.filter(static_routes=parent)
+
+
+@register_model_view(StaticRoute, name='edit')
 class StaticRouteEditView(ObjectEditView):
     queryset = StaticRoute.objects.all()
     form = StaticRouteForm
 
 
+@register_model_view(StaticRoute, name='delete')
 class StaticRouteDeleteView(ObjectDeleteView):
     pass
```

### Comparing `netbox-routing-0.0.1/netbox_routing.egg-info/PKG-INFO` & `netbox-routing-0.0.2/netbox_routing.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: netbox-routing
-Version: 0.0.1
+Version: 0.0.2
 Summary: NetBox Routing
 Home-page: https://github.com/dansheps/netbox-routing/
 Download-URL: https://pypi.org/project/netbox-routing/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
 License: All rights reserved
 Keywords: netbox,netbox-plugin
-Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 Plugin for documentation of routing configuration and objects
-
```

### Comparing `netbox-routing-0.0.1/netbox_routing.egg-info/SOURCES.txt` & `netbox-routing-0.0.2/netbox_routing.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -36,17 +36,20 @@
 netbox_routing/forms/fields.py
 netbox_routing/forms/objects.py
 netbox_routing/forms/static.py
 netbox_routing/forms/filtersets/__init__.py
 netbox_routing/forms/filtersets/objects.py
 netbox_routing/forms/filtersets/static.py
 netbox_routing/helpers/__init__.py
+netbox_routing/migrations/0001_initial.py
+netbox_routing/migrations/__init__.py
 netbox_routing/models/__init__.py
 netbox_routing/models/bgp.py
 netbox_routing/models/objects.py
+netbox_routing/models/ospf.py
 netbox_routing/models/static.py
 netbox_routing/tables/__init__.py
 netbox_routing/tables/objects.py
 netbox_routing/tables/static.py
 netbox_routing/templates/netbox_routing/staticroute.html
 netbox_routing/views/__init__.py
 netbox_routing/views/objects.py
```

### Comparing `netbox-routing-0.0.1/setup.py` & `netbox-routing-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-routing',
-    version='0.0.1',
+    version='0.0.2',
     description='NetBox Routing',
     long_description='Plugin for documentation of routing configuration and objects',
     url='https://github.com/dansheps/netbox-routing/',
     download_url='https://pypi.org/project/netbox-routing/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     maintainer='Daniel Sheppard',
@@ -15,13 +15,13 @@
     platform=[],
     keywords=['netbox', 'netbox-plugin'],
     classifiers=[
         'Framework :: Django',
         'Programming Language :: Python :: 3',
     ],
     install_requires=[
-        'importlib',
+        'django-polymorphic',
     ],
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
 )
```

