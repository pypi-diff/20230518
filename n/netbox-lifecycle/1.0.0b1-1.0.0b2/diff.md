# Comparing `tmp/netbox-lifecycle-1.0.0b1.tar.gz` & `tmp/netbox-lifecycle-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-lifecycle-1.0.0b1.tar", last modified: Thu May 11 02:08:50 2023, max compression
+gzip compressed data, was "netbox-lifecycle-1.0.0b2.tar", last modified: Thu May 18 03:16:41 2023, max compression
```

## Comparing `netbox-lifecycle-1.0.0b1.tar` & `netbox-lifecycle-1.0.0b2.tar`

### file list

```diff
@@ -1,62 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.861208 netbox-lifecycle-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-11 02:08:50.861208 netbox-lifecycle-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.853207 netbox-lifecycle-1.0.0b1/netbox_lifecycle/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.853207 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.853207 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/nested_serializers/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/nested_serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/nested_serializers/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/nested_serializers/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/nested_serializers/license.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.857207 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/serializers/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/serializers/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/serializers/license.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.857207 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/views/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/views/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/views/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/views/license.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.857207 netbox-lifecycle-1.0.0b1/netbox_lifecycle/filtersets/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/filtersets/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/filtersets/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/filtersets/license.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.857207 netbox-lifecycle-1.0.0b1/netbox_lifecycle/forms/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/forms/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/forms/model_forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.857207 netbox-lifecycle-1.0.0b1/netbox_lifecycle/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/migrations/0002_license_licenseassignment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.857207 netbox-lifecycle-1.0.0b1/netbox_lifecycle/models/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/models/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/models/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/models/license.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/models/netbox_polymprohic.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.861208 netbox-lifecycle-1.0.0b1/netbox_lifecycle/tables/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/tables/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/tables/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/tables/license.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.861208 netbox-lifecycle-1.0.0b1/netbox_lifecycle/views/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/views/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/views/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle/views/license.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 02:08:50.853207 netbox-lifecycle-1.0.0b1/netbox_lifecycle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-11 02:08:50.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-11 02:08:50.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 02:08:50.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 02:08:50.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 02:08:50.000000 netbox-lifecycle-1.0.0b1/netbox_lifecycle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 02:08:50.861208 netbox-lifecycle-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-11 02:08:44.000000 netbox-lifecycle-1.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.490361 netbox-lifecycle-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-18 03:16:41.490361 netbox-lifecycle-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.478360 netbox-lifecycle-1.0.0b2/netbox_lifecycle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.482360 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.482360 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/nested_serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/nested_serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/nested_serializers/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/nested_serializers/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/nested_serializers/license.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.482360 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/serializers/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/serializers/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/serializers/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.482360 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/views/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/views/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/views/license.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.482360 netbox-lifecycle-1.0.0b2/netbox_lifecycle/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/filtersets/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/filtersets/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/filtersets/license.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.486360 netbox-lifecycle-1.0.0b2/netbox_lifecycle/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/forms/bulk_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/forms/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/forms/model_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.486360 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0002_license_licenseassignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0003_remove_supportcontract_devices_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0004_supportcontractassignment_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0005_remove_supportcontract_manufacturer_supportsku_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0006_alter_supportcontractassignment_assigned_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0007_alter_hardwarelifecycle_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0008_alter_supportcontractassignment_contract_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0009_alter_licenseassignment_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0010_licenseassignment_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.486360 netbox-lifecycle-1.0.0b2/netbox_lifecycle/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/models/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/models/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/models/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/models/netbox_polymprohic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.486360 netbox-lifecycle-1.0.0b2/netbox_lifecycle/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/tables/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/tables/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/tables/license.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.478360 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.490361 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.490361 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/generic/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/hardwarelifecycle_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.490361 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/license/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/license/assignments.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/license.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.490361 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/supportcontract/assignments.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/supportcontract.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/supportcontractassignment_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/supportsku.html
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/templates/netbox_lifecycle/vendor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.490361 netbox-lifecycle-1.0.0b2/netbox_lifecycle/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/views/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/views/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle/views/license.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:16:41.482360 netbox-lifecycle-1.0.0b2/netbox_lifecycle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-18 03:16:41.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-18 03:16:41.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:16:41.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:16:41.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 03:16:41.000000 netbox-lifecycle-1.0.0b2/netbox_lifecycle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 03:16:41.490361 netbox-lifecycle-1.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-18 03:16:34.000000 netbox-lifecycle-1.0.0b2/setup.py
```

### Comparing `netbox-lifecycle-1.0.0b1/PKG-INFO` & `netbox-lifecycle-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-lifecycle
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: NetBox Lifecycle
 Home-page: https://github.com/dansheps/netbox-support-contract/
 Download-URL: https://github.com/dansheps/netbox-support-contract/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/nested_serializers/license.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/nested_serializers/license.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/serializers/hardware.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/serializers/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/serializers/license.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/serializers/license.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/views/contract.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/views/contract.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from rest_framework.viewsets import ModelViewSet
 
 from netbox_lifecycle.api.serializers import VendorSerializer, SupportContractSerializer, \
-    SupportContractDeviceAssignmentSerializer
-from netbox_lifecycle.models import Vendor, SupportContract, SupportContractDeviceAssignment
+    SupportContractAssignmentSerializer, SupportSKUSerializer
+from netbox_lifecycle.models import Vendor, SupportContract, SupportContractAssignment, SupportSKU
 
 __all__ = (
     'VendorViewSet',
+    'SupportSKUViewSet',
     'SupportContractViewSet',
-    'SupportContractDeviceAssignmentViewSet',
+    'SupportContractAssignmentViewSet',
 )
 
 
 class VendorViewSet(ModelViewSet):
     queryset = Vendor.objects.all()
     serializer_class = VendorSerializer
 
 
+class SupportSKUViewSet(ModelViewSet):
+    queryset = SupportSKU.objects.all()
+    serializer_class = SupportSKUSerializer
+
+
 class SupportContractViewSet(ModelViewSet):
     queryset = SupportContract.objects.all()
     serializer_class = SupportContractSerializer
 
 
-class SupportContractDeviceAssignmentViewSet(ModelViewSet):
-    queryset = SupportContractDeviceAssignment.objects.all()
-    serializer_class = SupportContractDeviceAssignmentSerializer
+class SupportContractAssignmentViewSet(ModelViewSet):
+    queryset = SupportContractAssignment.objects.all()
+    serializer_class = SupportContractAssignmentSerializer
```

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/api/views/license.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/api/views/license.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/forms/filtersets.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/forms/filtersets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from django.utils.translation import gettext as _
 from django.contrib.contenttypes.models import ContentType
 from django.db.models import Q
 
 from dcim.models import Device, Manufacturer
 from netbox.forms import NetBoxModelFilterSetForm
 from netbox_lifecycle.models import HardwareLifecycle, SupportContract, Vendor, License, LicenseAssignment, \
-    SupportContractDeviceAssignment
+    SupportContractAssignment, SupportSKU
+from utilities.filters import MultiValueCharFilter, MultiValueNumberFilter
 from utilities.forms.fields import DynamicModelMultipleChoiceField, TagFilterField
 from utilities.forms.widgets import APISelectMultiple
 
 
 __all__ = (
     'HardwareLifecycleFilterSetForm',
+    'SupportSKUFilterSetForm',
     'SupportContractFilterSetForm',
     'VendorFilterSetForm',
     'LicenseFilterSetForm',
     'LicenseAssignmentFilterSetForm',
-    'SupportContractDeviceAssignmentFilterSetForm'
+    'SupportContractAssignmentFilterSetForm'
 )
 
 
 class HardwareLifecycleFilterSetForm(NetBoxModelFilterSetForm):
     model = HardwareLifecycle
     fieldsets = (
         (None, ('q', 'filter_id', 'tag')),
@@ -33,27 +35,39 @@
         label=_('Object Type'),
         widget=APISelectMultiple(
             api_url='/api/extras/content-types/',
         )
     )
     tag = TagFilterField(model)
 
+    def search(self, queryset, name, value):
+        if not value.strip():
+            return queryset
 
-class SupportContractFilterSetForm(NetBoxModelFilterSetForm):
-    model = SupportContract
+
+class SupportSKUFilterSetForm(NetBoxModelFilterSetForm):
+    model = SupportSKU
     fieldsets = (
-        (None, ('q', 'filter_id', 'tag')),
-        ('Purchase Information', ('manufacturer_id', 'vendor_id', )),
+        (None, ('q', 'filter_id', 'tag', 'manufacturer_id')),
     )
     manufacturer_id = DynamicModelMultipleChoiceField(
         queryset=Manufacturer.objects.all(),
         required=False,
         selector=True,
         label=_('Manufacturer'),
     )
+    tag = TagFilterField(model)
+
+
+class SupportContractFilterSetForm(NetBoxModelFilterSetForm):
+    model = SupportContract
+    fieldsets = (
+        (None, ('q', 'filter_id', 'tag')),
+        ('Purchase Information', ('vendor_id', )),
+    )
     vendor_id = DynamicModelMultipleChoiceField(
         queryset=Vendor.objects.all(),
         required=False,
         selector=True,
         label=_('Vendor'),
     )
     tag = TagFilterField(model)
@@ -78,24 +92,30 @@
         required=False,
         selector=True,
         label=_('Manufacturer'),
     )
     tag = TagFilterField(model)
 
 
-class SupportContractDeviceAssignmentFilterSetForm(NetBoxModelFilterSetForm):
-    model = SupportContractDeviceAssignment
+class SupportContractAssignmentFilterSetForm(NetBoxModelFilterSetForm):
+    model = SupportContractAssignment
     fieldsets = (
         (None, ('q', 'filter_id', 'tag')),
-        ('Assignment', ('contract_id', 'device_id', )),
+        ('Assignment', ('contract_id', 'device_id', 'license_id', )),
     )
     contract_id = DynamicModelMultipleChoiceField(
         queryset=SupportContract.objects.all(),
         required=False,
         selector=True,
+        label=_('Contracts'),
+    )
+    license_id = DynamicModelMultipleChoiceField(
+        queryset=License.objects.all(),
+        required=False,
+        selector=True,
         label=_('Licenses'),
     )
     device_id = DynamicModelMultipleChoiceField(
         queryset=Device.objects.all(),
         required=False,
         selector=True,
         label=_('Devices'),
```

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/forms/model_forms.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/forms/model_forms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,163 @@
 from django import forms
 from django.utils.translation import gettext as _
 
 from dcim.models import DeviceType, ModuleType, Manufacturer, Device
 from netbox.forms import NetBoxModelForm
 from netbox_lifecycle.models import HardwareLifecycle, Vendor, SupportContract, LicenseAssignment, License, \
-    SupportContractDeviceAssignment
+    SupportContractAssignment, SupportSKU
 from utilities.forms.fields import DynamicModelChoiceField, DynamicModelMultipleChoiceField
 from utilities.forms.widgets import DatePicker
 
 
 __all__ = (
     'VendorForm',
+    'SupportSKUForm',
     'SupportContractForm',
-    'SupportContractDeviceAssignmentForm',
+    'SupportContractAssignmentForm',
     'LicenseForm',
     'LicenseAssignmentForm',
     'HardwareLifecycleForm'
 )
 
 
 class VendorForm(NetBoxModelForm):
 
     class Meta:
         model = Vendor
         fields = ('name', )
 
 
-class SupportContractForm(NetBoxModelForm):
+class SupportSKUForm(NetBoxModelForm):
     manufacturer = DynamicModelChoiceField(
         queryset=Manufacturer.objects.all(),
-        required=False,
         selector=False,
     )
+
+    class Meta:
+        model = SupportSKU
+        fields = ('manufacturer', 'sku', )
+
+
+class SupportContractForm(NetBoxModelForm):
     vendor = DynamicModelChoiceField(
         queryset=Vendor.objects.all(),
-        required=False,
         selector=True,
     )
 
     class Meta:
         model = SupportContract
-        fields = ('manufacturer', 'vendor', 'contract_id', 'start', 'renewal', 'end', )
+        fields = ('vendor', 'contract_id', 'start', 'renewal', 'end', )
         widgets = {
             'start': DatePicker(),
             'renewal': DatePicker(),
             'end': DatePicker(),
         }
 
 
-class SupportContractDeviceAssignmentForm(NetBoxModelForm):
+class SupportContractAssignmentForm(NetBoxModelForm):
     contract = DynamicModelChoiceField(
         queryset=SupportContract.objects.all(),
+        selector=True,
+    )
+    sku = DynamicModelChoiceField(
+        queryset=SupportSKU.objects.all(),
         required=False,
         selector=True,
+        label=_('SKU'),
     )
     device = DynamicModelChoiceField(
         queryset=Device.objects.all(),
         required=False,
         selector=True,
+        label=_('Device'),
+    )
+    license = DynamicModelChoiceField(
+        queryset=LicenseAssignment.objects.all(),
+        required=False,
+        selector=True,
+        label=_('License Assignment'),
     )
 
     class Meta:
-        model = SupportContractDeviceAssignment
-        fields = ('contract', 'device')
+        model = SupportContractAssignment
+        fields = ('contract', 'sku', 'device', 'license', 'end')
+        widgets = {
+            'end': DatePicker(),
+        }
+
+    def __init__(self, *args, **kwargs):
+
+        # Initialize helper selectors
+        instance = kwargs.get('instance')
+        initial = kwargs.get('initial', {}).copy()
+        if instance:
+            if type(instance.assigned_object) is Device:
+                initial['device'] = instance.assigned_object
+            elif type(instance.assigned_object) is LicenseAssignment:
+                initial['license'] = instance.assigned_object
+        kwargs['initial'] = initial
+
+        super().__init__(*args, **kwargs)
+
+    def clean(self):
+        super().clean()
+
+        # Handle object assignment
+        selected_objects = [
+            field for field in ('device', 'license') if self.cleaned_data[field]
+        ]
+
+        if len(selected_objects) > 1:
+            raise forms.ValidationError({
+                selected_objects[1]: "You can only assign a device or license"
+            })
+        elif selected_objects:
+            self.instance.assigned_object = self.cleaned_data[selected_objects[0]]
+        else:
+            self.instance.assigned_object = None
 
 
 class LicenseForm(NetBoxModelForm):
     manufacturer = DynamicModelChoiceField(
         queryset=Manufacturer.objects.all(),
-        required=False,
         selector=False,
     )
 
     class Meta:
         model = License
-        fields = ('name', 'manufacturer', )
+        fields = ('manufacturer', 'name', )
 
 
 class LicenseAssignmentForm(NetBoxModelForm):
     vendor = DynamicModelChoiceField(
         queryset=Vendor.objects.all(),
-        required=False,
         selector=True,
     )
     license = DynamicModelChoiceField(
         queryset=License.objects.all(),
-        required=False,
         selector=True,
     )
     device = DynamicModelChoiceField(
         queryset=Device.objects.all(),
         required=False,
         selector=True,
     )
 
     class Meta:
         model = LicenseAssignment
-        fields = ('vendor', 'license', 'device')
+        fields = ('vendor', 'license', 'device', 'quantity')
 
 
 class HardwareLifecycleForm(NetBoxModelForm):
     device_type = DynamicModelChoiceField(
         queryset=DeviceType.objects.all(),
         required=False,
         selector=True,
+        label=_('Device Type'),
     )
     module_type = DynamicModelChoiceField(
         queryset=ModuleType.objects.all(),
         required=False,
         selector=True,
         label=_('Module Type'),
     )
@@ -131,15 +181,15 @@
         # Initialize helper selectors
         instance = kwargs.get('instance')
         initial = kwargs.get('initial', {}).copy()
         if instance:
             if type(instance.assigned_object) is DeviceType:
                 initial['device_type'] = instance.assigned_object
             elif type(instance.assigned_object) is ModuleType:
-                initial['device_type'] = instance.assigned_object
+                initial['module_type'] = instance.assigned_object
         kwargs['initial'] = initial
 
         super().__init__(*args, **kwargs)
 
     def clean(self):
         super().clean()
```

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/migrations/0001_initial.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/migrations/0002_license_licenseassignment.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/migrations/0002_license_licenseassignment.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/models/hardware.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/models/hardware.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,14 +35,24 @@
     end_of_security = models.DateField(blank=True, null=True)
     last_contract_date = models.DateField(blank=True, null=True)
     end_of_support = models.DateField()
 
     notice = models.CharField(max_length=500, blank=True, null=True)
     documentation = models.CharField(max_length=500, blank=True, null=True)
 
+    class Meta:
+        ordering = ['assigned_object_type']
+        constraints = (
+            models.UniqueConstraint(
+                'assigned_object_type', 'assigned_object_id',
+                name='%(app_label)s_%(class)s_unique_object',
+                violation_error_message="Objects must be unique."
+            ),
+        )
+
     @property
     def name(self):
         return self
 
     def __str__(self):
         if isinstance(self.assigned_object, ModuleType):
             return f'Module Type: {self.assigned_object.model}'
```

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/tables/hardware.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/tables/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/tables/license.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/tables/license.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,12 +39,12 @@
     device = tables.Column(
         linkify=True
     )
 
     class Meta(NetBoxTable.Meta):
         model = LicenseAssignment
         fields = (
-            'pk', 'license', 'vendor', 'device'
+            'pk', 'license', 'vendor', 'device', 'quantity'
         )
         default_columns = (
             'pk', 'license', 'vendor', 'device'
         )
```

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/urls.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.urls import path
 
 from netbox.views.generic import ObjectChangeLogView
 from . import views
-from .models import HardwareLifecycle, SupportContract, License, LicenseAssignment, SupportContractDeviceAssignment
+from .models import HardwareLifecycle, SupportContract, License, LicenseAssignment, SupportContractAssignment, \
+    SupportSKU
 
 urlpatterns = [
     path('lifecycle/', views.HardwareLifecycleListView.as_view(), name='hardwarelifecycle_list'),
     path('lifecycle/add', views.HardwareLifecycleEditView.as_view(), name='hardwarelifecycle_add'),
     path('lifecycle/<int:pk>', views.HardwareLifecycleView.as_view(), name='hardwarelifecycle'),
     path('lifecycle/<int:pk>/edit', views.HardwareLifecycleEditView.as_view(), name='hardwarelifecycle_edit'),
     path('lifecycle/<int:pk>/delete', views.HardwareLifecycleDeleteView.as_view(), name='hardwarelifecycle_delete'),
@@ -18,31 +19,43 @@
     path('vendors/<int:pk>/edit', views.VendorEditView.as_view(), name='vendor_edit'),
     path('vendors/<int:pk>/delete', views.VendorDeleteView.as_view(), name='vendor_delete'),
     path('vendors/<int:pk>/changelog', ObjectChangeLogView.as_view(), name='vendor_changelog', kwargs={'model': SupportContract}),
 
     path('contracts/', views.SupportContractListView.as_view(), name='supportcontract_list'),
     path('contracts/add', views.SupportContractEditView.as_view(), name='supportcontract_add'),
     path('contracts/<int:pk>', views.SupportContractView.as_view(), name='supportcontract'),
-    path('contracts/<int:pk>/devices', views.SupportContractDeviceView.as_view(), name='supportcontract_devices'),
-    #path('contracts/<int:pk>/licenses', views.SupportContractLicenseView.as_view(), name='supportcontract_licenses'),
+    path('contracts/<int:pk>/devices', views.SupportContractAssignmentView.as_view(), name='supportcontract_assignments'),
     path('contracts/<int:pk>/edit', views.SupportContractEditView.as_view(), name='supportcontract_edit'),
     path('contracts/<int:pk>/delete', views.SupportContractDeleteView.as_view(), name='supportcontract_delete'),
     path('contracts/<int:pk>/changelog', ObjectChangeLogView.as_view(), name='supportcontract_changelog', kwargs={'model': SupportContract}),
 
-    path('contract_assignment/add', views.SupportContractDeviceAssignmentEditView.as_view(), name='supportcontractdeviceassignment_add'),
-    path('contract_assignment/<int:pk>/edit', views.SupportContractDeviceAssignmentEditView.as_view(), name='supportcontractdeviceassignment_edit'),
-    path('contract_assignment/<int:pk>/delete', views.SupportContractDeviceAssignmentDeleteView.as_view(), name='supportcontractdeviceassignment_delete'),
-    path('contract_assignment/<int:pk>/changelog', ObjectChangeLogView.as_view(), name='supportcontractdeviceassignment_changelog', kwargs={'model': SupportContractDeviceAssignment}),
+    path('contract-assignment/', views.SupportContractAssignmentListView.as_view(), name='supportcontractassignment_list'),
+    path('contract-assignment/add', views.SupportContractAssignmentEditView.as_view(), name='supportcontractassignment_add'),
+    path('contract-assignment/edit/', views.SupportContractAssignmentBulkEditView.as_view(), name='supportcontractassignment_bulk_edit'),
+    path('contract-assignment/delete/', views.SupportContractAssignmentBulkDeleteView.as_view(), name='supportcontractassignment_bulk_delete'),
+    path('contract-assignment/<int:pk>/edit', views.SupportContractAssignmentEditView.as_view(), name='supportcontractassignment_edit'),
+    path('contract-assignment/<int:pk>/delete', views.SupportContractAssignmentDeleteView.as_view(), name='supportcontractassignment_delete'),
+    path('contract-assignment/<int:pk>/changelog', ObjectChangeLogView.as_view(), name='supportcontractassignment_changelog', kwargs={'model': SupportContractAssignment}),
 
     path('license/', views.LicenseListView.as_view(), name='license_list'),
     path('license/add', views.LicenseEditView.as_view(), name='license_add'),
     path('license/<int:pk>', views.LicenseView.as_view(), name='license'),
     path('license/<int:pk>/assignments', views.LicenseAssignmentView.as_view(), name='license_assignments'),
     path('license/<int:pk>/edit', views.LicenseEditView.as_view(), name='license_edit'),
     path('license/<int:pk>/delete', views.LicenseDeleteView.as_view(), name='license_delete'),
     path('license/<int:pk>/changelog', ObjectChangeLogView.as_view(), name='license_changelog', kwargs={'model': License}),
 
-    path('license_assignment/add', views.LicenseAssignmentEditView.as_view(), name='licenseassignment_add'),
-    path('license_assignment/<int:pk>/edit', views.LicenseAssignmentEditView.as_view(), name='licenseassignment_edit'),
-    path('license_assignment/<int:pk>/delete', views.LicenseAssignmentDeleteView.as_view(), name='licenseassignment_delete'),
-    path('license_assignment/<int:pk>/changelog', ObjectChangeLogView.as_view(), name='licenseassignment_changelog', kwargs={'model': LicenseAssignment}),
+    path('sku/', views.SupportSKUListView.as_view(), name='supportsku_list'),
+    path('sku/add', views.SupportSKUEditView.as_view(), name='supportsku_add'),
+    path('sku/<int:pk>', views.SupportSKUView.as_view(), name='supportsku'),
+    path('sku/<int:pk>/edit', views.SupportSKUEditView.as_view(), name='supportsku_edit'),
+    path('sku/<int:pk>/delete', views.SupportSKUDeleteView.as_view(), name='supportsku_delete'),
+    path('sku/<int:pk>/changelog', ObjectChangeLogView.as_view(), name='supportsku_changelog', kwargs={'model': SupportSKU}),
+
+    path('license-assignment/', views.LicenseAssignmentListView.as_view(), name='licenseassignment_list'),
+    path('license-assignment/add', views.LicenseAssignmentEditView.as_view(), name='licenseassignment_add'),
+    path('license-assignment/<int:pk>/edit', views.LicenseAssignmentEditView.as_view(), name='licenseassignment_edit'),
+    path('license-assignment/<int:pk>/delete', views.LicenseAssignmentDeleteView.as_view(), name='licenseassignment_delete'),
+    path('license-assignment/<int:pk>/changelog', ObjectChangeLogView.as_view(), name='licenseassignment_changelog', kwargs={'model': LicenseAssignment}),
+    path('license-assignment/delete/', views.LicenseAssignmentBulkDeleteView.as_view(), name='licenseassignment_bulk_delete'),
+    path('license-assignment/<int:pk>/edit', views.LicenseAssignmentEditView.as_view(), name='licenseassignment_edit'),
 ]
```

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/views/hardware.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/views/hardware.py`

 * *Files identical despite different names*

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle/views/license.py` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle/views/license.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-from netbox.views.generic import ObjectListView, ObjectEditView, ObjectDeleteView, ObjectView, ObjectChildrenView
+from netbox.views.generic import ObjectListView, ObjectEditView, ObjectDeleteView, ObjectView, ObjectChildrenView, \
+    BulkEditView, BulkDeleteView
 from netbox_lifecycle.filtersets import LicenseFilterSet, LicenseAssignmentFilterSet
-from netbox_lifecycle.forms import LicenseFilterSetForm, LicenseForm, LicenseAssignmentForm
+from netbox_lifecycle.forms import LicenseFilterSetForm, LicenseForm, LicenseAssignmentForm, \
+    LicenseAssignmentBulkEditForm, LicenseAssignmentFilterSetForm
 from netbox_lifecycle.models import License, LicenseAssignment
 from netbox_lifecycle.tables import LicenseTable, LicenseAssignmentTable
 from utilities.views import ViewTab, register_model_view
 
 
 __all__ = (
     'LicenseListView',
     'LicenseView',
     'LicenseEditView',
     'LicenseDeleteView',
     'LicenseAssignmentView',
+    'LicenseAssignmentListView',
     'LicenseAssignmentEditView',
     'LicenseAssignmentDeleteView',
+    'LicenseAssignmentBulkEditView',
+    'LicenseAssignmentBulkDeleteView',
 )
 
 @register_model_view(License, name='list')
 class LicenseListView(ObjectListView):
     queryset = License.objects.all()
     table = LicenseTable
     filterset = LicenseFilterSet
@@ -36,15 +41,14 @@
 
 
 @register_model_view(License, 'delete')
 class LicenseDeleteView(ObjectDeleteView):
     queryset = License.objects.all()
 
 
-
 @register_model_view(License, 'assignments')
 class LicenseAssignmentView(ObjectChildrenView):
     template_name = 'netbox_lifecycle/license/assignments.html'
     queryset = License.objects.all()
     child_model = LicenseAssignment
     table = LicenseAssignmentTable
     filterset = LicenseAssignmentFilterSet
@@ -55,17 +59,37 @@
         badge=lambda obj: LicenseAssignment.objects.filter(license=obj).count(),
     )
 
     def get_children(self, request, parent):
         return self.child_model.objects.filter(license=parent)
 
 
+@register_model_view(LicenseAssignment, name='list')
+class LicenseAssignmentListView(ObjectListView):
+    queryset = LicenseAssignment.objects.all()
+    table = LicenseAssignmentTable
+    filterset = LicenseAssignmentFilterSet
+    filterset_form = LicenseAssignmentFilterSetForm
+
+
 @register_model_view(LicenseAssignment, 'edit')
 class LicenseAssignmentEditView(ObjectEditView):
     queryset = LicenseAssignment.objects.all()
     form = LicenseAssignmentForm
 
 
 @register_model_view(LicenseAssignment, 'delete')
 class LicenseAssignmentDeleteView(ObjectDeleteView):
     queryset = LicenseAssignment.objects.all()
 
+
+class LicenseAssignmentBulkEditView(BulkEditView):
+    queryset = LicenseAssignment.objects.all()
+    filterset = LicenseAssignmentFilterSet
+    table = LicenseAssignmentTable
+    form = LicenseAssignmentBulkEditForm
+
+
+class LicenseAssignmentBulkDeleteView(BulkDeleteView):
+    queryset = LicenseAssignment.objects.all()
+    filterset = LicenseAssignmentFilterSet
+    table = LicenseAssignmentTable
```

### Comparing `netbox-lifecycle-1.0.0b1/netbox_lifecycle.egg-info/PKG-INFO` & `netbox-lifecycle-1.0.0b2/netbox_lifecycle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-lifecycle
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: NetBox Lifecycle
 Home-page: https://github.com/dansheps/netbox-support-contract/
 Download-URL: https://github.com/dansheps/netbox-support-contract/
 Author: Daniel Sheppard
 Author-email: dans@dansheps.com
 Maintainer: Daniel Sheppard
 Maintainer-email: dans@dansheps.com
```

### Comparing `netbox-lifecycle-1.0.0b1/setup.py` & `netbox-lifecycle-1.0.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-lifecycle',
-    version='1.0.0-beta1',
+    version='1.0.0-beta2',
     description='NetBox Lifecycle',
     long_description='NetBox Support Contract and EOL/EOS management',
     url='https://github.com/dansheps/netbox-support-contract/',
     download_url='https://github.com/dansheps/netbox-support-contract/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     maintainer='Daniel Sheppard',
```

