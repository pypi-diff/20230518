# Comparing `tmp/pyatlan-0.0.31.tar.gz` & `tmp/pyatlan-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.0.31.tar", last modified: Mon May 15 11:10:35 2023, max compression
+gzip compressed data, was "pyatlan-0.0.32.tar", last modified: Thu May 18 17:20:32 2023, max compression
```

## Comparing `pyatlan-0.0.31.tar` & `pyatlan-0.0.32.tar`

### file list

```diff
@@ -1,67 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.751690 pyatlan-0.0.31/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-15 11:10:21.000000 pyatlan-0.0.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 11:10:21.000000 pyatlan-0.0.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-15 11:10:21.000000 pyatlan-0.0.31/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-15 11:10:35.751690 pyatlan-0.0.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-15 11:10:21.000000 pyatlan-0.0.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.739690 pyatlan-0.0.31/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.739690 pyatlan-0.0.31/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/cache/role_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.739690 pyatlan-0.0.31/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26718 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.743690 pyatlan-0.0.31/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.743690 pyatlan-0.0.31/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.747690 pyatlan-0.0.31/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   869422 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    58716 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16624 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 11:10:21.000000 pyatlan-0.0.31/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.739690 pyatlan-0.0.31/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 11:10:35.000000 pyatlan-0.0.31/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:10:35.751690 pyatlan-0.0.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-15 11:10:21.000000 pyatlan-0.0.31/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.747690 pyatlan-0.0.31/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.747690 pyatlan-0.0.31/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/role_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33620 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/test_entity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/integration/test_index_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:10:35.747690 pyatlan-0.0.31/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    57228 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-15 11:10:21.000000 pyatlan-0.0.31/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.792536 pyatlan-0.0.32/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-18 17:20:21.000000 pyatlan-0.0.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 17:20:21.000000 pyatlan-0.0.32/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-18 17:20:21.000000 pyatlan-0.0.32/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-18 17:20:32.792536 pyatlan-0.0.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-18 17:20:21.000000 pyatlan-0.0.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.784536 pyatlan-0.0.32/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/cache/role_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34780 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   958128 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 17:20:21.000000 pyatlan-0.0.32/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.784536 pyatlan-0.0.32/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 17:20:32.000000 pyatlan-0.0.32/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:20:32.792536 pyatlan-0.0.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-18 17:20:21.000000 pyatlan-0.0.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.788536 pyatlan-0.0.32/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.792536 pyatlan-0.0.32/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35863 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34056 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/test_entity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/integration/test_index_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:20:32.792536 pyatlan-0.0.32/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64373 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-18 17:20:21.000000 pyatlan-0.0.32/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.0.31/LICENSE` & `pyatlan-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.31/PKG-INFO` & `pyatlan-0.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.31
+Version: 0.0.32
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.31/README.md` & `pyatlan-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.31/pyatlan/cache/classification_cache.py` & `pyatlan-0.0.32/pyatlan/cache/classification_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Optional
 
 from pyatlan.model.enums import AtlanTypeCategory
 from pyatlan.model.typedef import ClassificationDef
 
 
 class ClassificationCache:
-
     cache_by_id: dict[str, ClassificationDef] = dict()
     map_id_to_name: dict[str, str] = dict()
     map_name_to_id: dict[str, str] = dict()
     deleted_ids: set[str] = set()
     deleted_names: set[str] = set()
 
     @classmethod
```

### Comparing `pyatlan-0.0.31/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.0.32/pyatlan/cache/custom_metadata_cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 import json
 from typing import Any, Optional
 
 from pyatlan.client.atlan import AtlanClient
-from pyatlan.error import LogicError, NotFoundError
+from pyatlan.error import InvalidRequestError, LogicError, NotFoundError
 from pyatlan.model.core import CustomMetadata
 from pyatlan.model.enums import AtlanTypeCategory
 from pyatlan.model.typedef import AttributeDef, CustomMetadataDef
 
 
 class Synonym:
     def __init__(self, storage_name):
@@ -20,15 +20,14 @@
     def __get__(self, instance, owner):
         if self.storage_name in instance:
             return instance[self.storage_name]
         return None
 
 
 class CustomMetadataCache:
-
     cache_by_id: dict[str, CustomMetadataDef] = dict()
     map_id_to_name: dict[str, str] = dict()
     map_id_to_type: dict[str, type] = dict()
     map_name_to_id: dict[str, str] = dict()
     map_attr_id_to_name: dict[str, dict[str, str]] = dict()
     map_attr_name_to_id: dict[str, dict[str, str]] = dict()
     archived_attr_ids: dict[str, str] = dict()
@@ -62,59 +61,82 @@
                 attrib_type = type(attribute_class_name, (CustomMetadata,), {})
                 attrib_type._meta_data_type_id = type_id  # type: ignore
                 attrib_type._meta_data_type_name = type_name  # type: ignore
                 cls.map_id_to_type[type_id] = attrib_type
                 applicable_types: set[str] = set()
                 if cm.attribute_defs:
                     for attr in cm.attribute_defs:
-                        if attr.options.custom_applicable_entity_types:
+                        if attr.options and attr.options.custom_applicable_entity_types:
                             applicable_types.update(
                                 json.loads(attr.options.custom_applicable_entity_types)
                             )
-                        attr_id = attr.name
-                        attr_name = attr.display_name
-                        cls.map_attr_id_to_name[type_id][attr_id] = attr_name
+                        attr_id = str(attr.name)
+                        attr_name = str(attr.display_name)
+                        # Use a renamed attribute everywhere
+                        attr_renamed = to_snake_case(attr_name)
+                        cls.map_attr_id_to_name[type_id][attr_id] = attr_renamed
                         if attr.options and attr.options.is_archived:
-                            cls.archived_attr_ids[attr_id] = attr_name
-                        elif attr_name in cls.map_attr_name_to_id[type_id]:
+                            cls.archived_attr_ids[attr_id] = attr_renamed
+                        elif attr_renamed in cls.map_attr_name_to_id[type_id]:
                             raise LogicError(
-                                f"Multiple custom attributes with exactly the same name ({attr_name}) "
+                                f"Multiple custom attributes with exactly the same name ({attr_renamed}) "
                                 f"found for: {type_name}",
                                 code="ATLAN-PYTHON-500-100",
                             )
                         else:
-                            attr_name = to_snake_case(attr_name.replace(" ", ""))
-                            setattr(attrib_type, attr_name, Synonym(attr_id))
-                            cls.map_attr_name_to_id[type_id][attr_name] = attr_id
+                            setattr(attrib_type, attr_renamed, Synonym(attr_id))
+                            cls.map_attr_name_to_id[type_id][attr_renamed] = attr_id
                     for asset_type in applicable_types:
                         if asset_type not in cls.types_by_asset:
                             cls.types_by_asset[asset_type] = set()
                         cls.types_by_asset[asset_type].add(attrib_type)
 
     @classmethod
-    def get_id_for_name(cls, name: str) -> Optional[str]:
+    def get_id_for_name(cls, name: str) -> str:
         """
         Translate the provided human-readable custom metadata set name to its Atlan-internal ID string.
         """
+        if name is None or not name.strip():
+            raise InvalidRequestError(
+                message="No name was provided when attempting to retrieve custom metadata.",
+                code="ATLAN-PYTHON-404-008",
+                param="",
+            )
         if cm_id := cls.map_name_to_id.get(name):
             return cm_id
         # If not found, refresh the cache and look again (could be stale)
         cls.refresh_cache()
-        return cls.map_name_to_id.get(name)
+        if cm_id := cls.map_name_to_id.get(name):
+            return cm_id
+        raise NotFoundError(
+            message=f"Custom metadata with name {name} does not exist.",
+            code="ATLAN-PYTHON-404-009",
+        )
 
     @classmethod
-    def get_name_for_id(cls, idstr: str) -> Optional[str]:
+    def get_name_for_id(cls, idstr: str) -> str:
         """
         Translate the provided Atlan-internal custom metadata ID string to the human-readable custom metadata set name.
         """
+        if idstr is None or not idstr.strip():
+            raise InvalidRequestError(
+                message="No ID was provided when attempting to retrieve custom metadata.",
+                code="ATLAN-PYTHON-404-008",
+                param="",
+            )
         if cm_name := cls.map_id_to_name.get(idstr):
             return cm_name
         # If not found, refresh the cache and look again (could be stale)
         cls.refresh_cache()
-        return cls.map_id_to_name.get(idstr)
+        if cm_name := cls.map_id_to_name.get(idstr):
+            return cm_name
+        raise NotFoundError(
+            message=f"Custom metadata with ID {idstr} does not exist.",
+            code="ATLAN-PYTHON-404-009",
+        )
 
     @classmethod
     def get_type_for_id(cls, idstr: str) -> Optional[type]:
         if cm_type := cls.map_id_to_type.get(idstr):
             return cm_type
         cls.refresh_cache()
         return cls.map_id_to_type.get(idstr)
@@ -148,41 +170,49 @@
                         for attr in attribute_defs
                         if not attr.options or not attr.options.is_archived
                     )
             m[type_name] = to_include
         return m
 
     @classmethod
-    def get_attr_id_for_name(cls, set_name: str, attr_name: str) -> Optional[str]:
+    def get_attr_id_for_name(cls, set_name: str, attr_name: str) -> str:
         """
         Translate the provided human-readable custom metadata set and attribute names to the Atlan-internal ID string
         for the attribute.
         """
-        attr_id = None
-        if set_id := cls.get_id_for_name(set_name):
-            if sub_map := cls.map_attr_name_to_id.get(set_id):
-                attr_id = sub_map.get(attr_name)
+        set_id = cls.get_id_for_name(set_name)
+        if sub_map := cls.map_attr_name_to_id.get(set_id):
+            attr_id = sub_map.get(attr_name)
             if attr_id:
                 # If found, return straight away
                 return attr_id
-            # Otherwise, refresh the cache and look again (could be stale)
-            cls.refresh_cache()
-            if sub_map := cls.map_attr_name_to_id.get(set_id):
-                return sub_map.get(attr_name)
-        return None
+        # Otherwise, refresh the cache and look again (could be stale)
+        cls.refresh_cache()
+        if sub_map := cls.map_attr_name_to_id.get(set_id):
+            attr_id = sub_map.get(attr_name)
+            if attr_id:
+                # If found, return straight away
+                return attr_id
+            raise NotFoundError(
+                message=f"Custom metadata property with name {attr_name} does not exist in custom metadata {set_name}.",
+                code="ATLAN-PYTHON-404-009",
+            )
+        raise NotFoundError(
+            message=f"Custom metadata with ID {set_id} does not exist.",
+            code="ATLAN-PYTHON-404-009",
+        )
 
     @classmethod
     def get_attr_name_for_id(cls, set_id: str, attr_id: str) -> Optional[str]:
         """
         Translate the provided human-readable custom metadata set and attribute names to the Atlan-internal ID string
         for the attribute.
         """
         if sub_map := cls.map_attr_id_to_name.get(set_id):
-            attr_name = sub_map.get(attr_id)
-            if attr_name:
+            if attr_name := sub_map.get(attr_id):
                 return attr_name
             cls.refresh_cache()
             if sub_map := cls.map_attr_id_to_name.get(set_id):
                 return sub_map.get(attr_id)
         return None
 
     @classmethod
@@ -226,7 +256,20 @@
         if ba_type := CustomMetadataCache.get_type_for_id(ba_id):
             return (
                 ba_type(business_attributes[ba_id])
                 if business_attributes and ba_id in business_attributes
                 else ba_type()
             )
         raise ValueError(f"Custom metadata {name} is not applicable to {type_name}")
+
+    @classmethod
+    def get_custom_metadata_def(cls, name: str) -> CustomMetadataDef:
+        """
+        Retrieve the full custom metadata structure definition.
+        """
+        ba_id = cls.get_id_for_name(name)
+        if ba_id is None:
+            raise ValueError(f"No custom metadata with the name: {name} exist")
+        if typedef := cls.cache_by_id.get(ba_id):
+            return typedef
+        else:
+            raise ValueError(f"No custom metadata with the name: {name} found")
```

### Comparing `pyatlan-0.0.31/pyatlan/cache/role_cache.py` & `pyatlan-0.0.32/pyatlan/cache/role_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Optional
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.role import AtlanRole
 
 
 class RoleCache:
-
     cache_by_id: dict[str, AtlanRole] = dict()
     map_id_to_name: dict[str, str] = dict()
     map_name_to_id: dict[str, str] = dict()
 
     @classmethod
     def _refresh_cache(cls) -> None:
         client = AtlanClient.get_default_client()
```

### Comparing `pyatlan-0.0.31/pyatlan/client/atlan.py` & `pyatlan-0.0.32/pyatlan/client/atlan.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,25 +19,30 @@
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from pyatlan.client.constants import (
     ADD_BUSINESS_ATTRIBUTE_BY_ID,
     BULK_UPDATE,
     CREATE_TYPE_DEFS,
+    UPDATE_TYPE_DEFS,
     DELETE_ENTITY_BY_ATTRIBUTE,
     DELETE_ENTITY_BY_GUID,
     DELETE_TYPE_DEF_BY_NAME,
     GET_ALL_TYPE_DEFS,
     GET_ENTITY_BY_GUID,
     GET_ENTITY_BY_UNIQUE_ATTRIBUTE,
     GET_LINEAGE,
     GET_ROLES,
+    GET_GROUPS,
     INDEX_SEARCH,
     PARTIAL_UPDATE_ENTITY_BY_ATTRIBUTE,
     UPDATE_ENTITY_BY_ATTRIBUTE,
+    CREATE_GROUP,
+    DELETE_GROUP,
+    UPDATE_GROUP,
 )
 from pyatlan.error import AtlanError, NotFoundError
 from pyatlan.exceptions import AtlanServiceException, InvalidRequestException
 from pyatlan.model.assets import (
     Asset,
     AtlasGlossary,
     AtlasGlossaryCategory,
@@ -64,14 +69,20 @@
 )
 from pyatlan.model.enums import (
     AtlanConnectorType,
     AtlanDeleteType,
     AtlanTypeCategory,
     CertificateStatus,
 )
+from pyatlan.model.group import (
+    GroupResponse,
+    AtlanGroup,
+    CreateGroupResponse,
+    CreateGroupRequest,
+)
 from pyatlan.model.lineage import LineageRequest, LineageResponse
 from pyatlan.model.response import AssetMutationResponse
 from pyatlan.model.role import RoleResponse
 from pyatlan.model.search import DSL, IndexSearchRequest, Term
 from pyatlan.model.typedef import (
     ClassificationDef,
     CustomMetadataDef,
@@ -118,14 +129,69 @@
     adapter = HTTPAdapter(max_retries=retry_strategy)
     session = requests.session()
     session.mount("https://", adapter)
     session.headers.update({"x-atlan-agent": "sdk", "x-atlan-agent-id": "python"})
     return session
 
 
+def _build_typedef_request(typedef: TypeDef) -> TypeDefResponse:
+    if isinstance(typedef, ClassificationDef):
+        # Set up the request payload...
+        payload = TypeDefResponse(
+            classification_defs=[typedef],
+            enum_defs=[],
+            struct_defs=[],
+            entity_defs=[],
+            relationship_defs=[],
+            custom_metadata_defs=[],
+        )
+    elif isinstance(typedef, CustomMetadataDef):
+        # Set up the request payload...
+        payload = TypeDefResponse(
+            classification_defs=[],
+            enum_defs=[],
+            struct_defs=[],
+            entity_defs=[],
+            relationship_defs=[],
+            custom_metadata_defs=[typedef],
+        )
+    elif isinstance(typedef, EnumDef):
+        # Set up the request payload...
+        payload = TypeDefResponse(
+            classification_defs=[],
+            enum_defs=[typedef],
+            struct_defs=[],
+            entity_defs=[],
+            relationship_defs=[],
+            custom_metadata_defs=[],
+        )
+    else:
+        raise InvalidRequestException(
+            "Unable to update type definitions of category: " + typedef.category.value,
+            param="category",
+        )
+        # Throw an invalid request exception
+    return payload
+
+
+def _refresh_caches(typedef: TypeDef) -> None:
+    if isinstance(typedef, ClassificationDef):
+        from pyatlan.cache.classification_cache import ClassificationCache
+
+        ClassificationCache.refresh_cache()
+    if isinstance(typedef, CustomMetadataDef):
+        from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+
+        CustomMetadataCache.refresh_cache()
+    if isinstance(typedef, EnumDef):
+        from pyatlan.cache.enum_cache import EnumCache
+
+        EnumCache.refresh_cache()
+
+
 class AtlanClient(BaseSettings):
     _default_client: "ClassVar[Optional[AtlanClient]]" = None
     base_url: HttpUrl
     api_key: str
     _session: requests.Session = PrivateAttr(default_factory=get_session)
     _request_params: dict = PrivateAttr()
 
@@ -203,14 +269,16 @@
             LOGGER.debug("HTTP Status: %s", response.status_code)
         if response is None:
             return None
         if response.status_code == api.expected_status:
             try:
                 if (
                     response.content is None
+                    or response.content == "null"
+                    or len(response.content) == 0
                     or response.status_code == HTTPStatus.NO_CONTENT
                 ):
                     return None
                 if LOGGER.isEnabledFor(logging.DEBUG):
                     LOGGER.debug(
                         "<== __call_api(%s,%s,%s), result = %s",
                         vars(api),
@@ -230,15 +298,15 @@
             LOGGER.error(
                 "Atlas Service unavailable. HTTP Status: %s",
                 HTTPStatus.SERVICE_UNAVAILABLE,
             )
 
             return None
         else:
-            with contextlib.suppress(ValueError):
+            with contextlib.suppress(ValueError, json.decoder.JSONDecodeError):
                 error_info = json.loads(response.text)
                 error_code = error_info.get("errorCode", 0)
                 error_message = error_info.get("errorMessage", "")
                 if error_code and error_message:
                     raise AtlanError(
                         message=error_message,
                         code=error_code,
@@ -294,14 +362,96 @@
     def get_all_roles(self) -> RoleResponse:
         """
         Retrieve all roles defined in Atlan.
         """
         raw_json = self._call_api(GET_ROLES.format_path_with_params())
         return RoleResponse(**raw_json)
 
+    def create_group(
+        self,
+        group: AtlanGroup,
+        user_ids: Optional[list[str]] = None,
+    ) -> CreateGroupResponse:
+        payload = CreateGroupRequest(group=group, user_ids=user_ids)
+        raw_json = self._call_api(CREATE_GROUP, request_obj=payload, exclude_unset=True)
+        return CreateGroupResponse(**raw_json)
+
+    def update_group(
+        self,
+        group: AtlanGroup,
+    ) -> None:
+        self._call_api(
+            UPDATE_GROUP.format_path_with_params(group.id),
+            request_obj=group,
+            exclude_unset=True,
+        )
+
+    def purge_group(
+        self,
+        guid: str,
+    ) -> None:
+        self._call_api(DELETE_GROUP.format_path({"group_guid": guid}))
+
+    def get_groups(
+        self,
+        limit: Optional[int] = None,
+        post_filter: Optional[str] = None,
+        sort: Optional[str] = None,
+        count: bool = True,
+        offset: int = 0,
+    ) -> GroupResponse:
+        query_params: dict[str, str] = {
+            "count": str(count),
+            "offset": str(offset),
+        }
+        if limit is not None:
+            query_params["limit"] = str(limit)
+        if post_filter is not None:
+            query_params["filter"] = post_filter
+        if sort is not None:
+            query_params["sort"] = sort
+        raw_json = self._call_api(GET_GROUPS.format_path_with_params(), query_params)
+        return GroupResponse(**raw_json)
+
+    def get_all_groups(self) -> list[AtlanGroup]:
+        """
+        Retrieve all groups defined in Atlan.
+        """
+        groups: list[AtlanGroup] = []
+        offset = 0
+        limit = 100
+        response: Optional[GroupResponse] = self.get_groups(
+            offset=offset, limit=limit, sort="createdAt"
+        )
+        while response:
+            if page := response.records:
+                groups.extend(page)
+                offset += limit
+                response = self.get_groups(offset=offset, limit=limit, sort="createdAt")
+            else:
+                response = None
+        return groups
+
+    def get_group_by_name(
+        self, alias: str, limit: int = 100
+    ) -> Optional[list[AtlanGroup]]:
+        """
+        Retrieve all groups with a name that contains the provided string.
+        (This could include a complete group name, in which case there should be at most
+        a single item in the returned list, or could be a partial group name to retrieve
+        all groups with that naming convention.)
+        """
+        if response := self.get_groups(
+            offset=0,
+            limit=limit,
+            post_filter='{"$and":[{"alias":{"$ilike":"%' + alias + '%"}}]}',
+        ):
+            return response.records
+        return None
+
     @validate_arguments()
     def get_asset_by_qualified_name(
         self,
         qualified_name: str,
         asset_type: Type[A],
         min_ext_info: bool = False,
         ignore_relationships: bool = False,
@@ -405,14 +555,52 @@
             entities.append(entity)
         for asset in entities:
             asset.validate_required()
         request = BulkRequest[Asset](entities=entities)
         raw_json = self._call_api(BULK_UPDATE, query_params, request)
         return AssetMutationResponse(**raw_json)
 
+    def upsert_merging_cm(
+        self, entity: Union[Asset, list[Asset]], replace_classifications: bool = False
+    ) -> AssetMutationResponse:
+        query_params = {
+            "replaceClassifications": replace_classifications,
+            "replaceBusinessAttributes": True,
+            "overwriteBusinessAttributes": False,
+        }
+        entities: list[Asset] = []
+        if isinstance(entity, list):
+            entities.extend(entity)
+        else:
+            entities.append(entity)
+        for asset in entities:
+            asset.validate_required()
+        request = BulkRequest[Asset](entities=entities)
+        raw_json = self._call_api(BULK_UPDATE, query_params, request)
+        return AssetMutationResponse(**raw_json)
+
+    def upsert_replacing_cm(
+        self, entity: Union[Asset, list[Asset]], replace_classifications: bool = False
+    ) -> AssetMutationResponse:
+        query_params = {
+            "replaceClassifications": replace_classifications,
+            "replaceBusinessAttributes": True,
+            "overwriteBusinessAttributes": True,
+        }
+        entities: list[Asset] = []
+        if isinstance(entity, list):
+            entities.extend(entity)
+        else:
+            entities.append(entity)
+        for asset in entities:
+            asset.validate_required()
+        request = BulkRequest[Asset](entities=entities)
+        raw_json = self._call_api(BULK_UPDATE, query_params, request)
+        return AssetMutationResponse(**raw_json)
+
     def purge_entity_by_guid(self, guid) -> AssetMutationResponse:
         raw_json = self._call_api(
             DELETE_ENTITY_BY_GUID.format_path_with_params(guid),
             {"deleteType": AtlanDeleteType.HARD.value},
         )
         return AssetMutationResponse(**raw_json)
 
@@ -451,70 +639,67 @@
         raw_json = self._call_api(
             GET_ALL_TYPE_DEFS.format_path_with_params(),
             query_params,
         )
         return TypeDefResponse(**raw_json)
 
     def create_typedef(self, typedef: TypeDef) -> TypeDefResponse:
-        if isinstance(typedef, ClassificationDef):
-            # Set up the request payload...
-            payload = TypeDefResponse(
-                classification_defs=[typedef],
-                enum_defs=[],
-                struct_defs=[],
-                entity_defs=[],
-                relationship_defs=[],
-                custom_metadata_defs=[],
-            )
-        elif isinstance(typedef, CustomMetadataDef):
-            # Set up the request payload...
-            payload = TypeDefResponse(
-                classification_defs=[],
-                enum_defs=[],
-                struct_defs=[],
-                entity_defs=[],
-                relationship_defs=[],
-                custom_metadata_defs=[typedef],
-            )
-        elif isinstance(typedef, EnumDef):
-            # Set up the request payload...
-            payload = TypeDefResponse(
-                classification_defs=[],
-                enum_defs=[typedef],
-                struct_defs=[],
-                entity_defs=[],
-                relationship_defs=[],
-                custom_metadata_defs=[],
-            )
+        payload = _build_typedef_request(typedef)
+        raw_json = self._call_api(
+            CREATE_TYPE_DEFS, request_obj=payload, exclude_unset=True
+        )
+        _refresh_caches(typedef)
+        return TypeDefResponse(**raw_json)
+
+    def update_typedef(self, typedef: TypeDef) -> TypeDefResponse:
+        payload = _build_typedef_request(typedef)
+        raw_json = self._call_api(
+            UPDATE_TYPE_DEFS, request_obj=payload, exclude_unset=True
+        )
+        _refresh_caches(typedef)
+        return TypeDefResponse(**raw_json)
+
+    def purge_typedef(self, name: str, typedef_type: type) -> None:
+        if typedef_type == CustomMetadataDef:
+            from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+
+            internal_name = CustomMetadataCache.get_id_for_name(name)
+        elif typedef_type == EnumDef:
+            internal_name = name
+        elif typedef_type == ClassificationDef:
+            from pyatlan.cache.classification_cache import ClassificationCache
+
+            internal_name = str(ClassificationCache.get_id_for_name(name))
         else:
             raise InvalidRequestException(
-                "Unable to create new type definitions of category: "
-                + typedef.category.value,
-                param="category",
+                message=f"Unable to purge type definitions of type: {typedef_type}",
             )
             # Throw an invalid request exception
-        raw_json = self._call_api(
-            CREATE_TYPE_DEFS, request_obj=payload, exclude_unset=False
-        )
-        if isinstance(typedef, ClassificationDef):
-            from pyatlan.cache.classification_cache import ClassificationCache
-            ClassificationCache.refresh_cache()
-        if isinstance(typedef, CustomMetadataDef):
+        if internal_name:
+            self._call_api(
+                DELETE_TYPE_DEF_BY_NAME.format_path_with_params(internal_name)
+            )
+        else:
+            raise NotFoundError(
+                message=f"Unable to find {typedef_type} with name: {name}",
+                code="ATLAN-PYTHON-404-000",
+            )
+
+        if typedef_type == CustomMetadataDef:
             from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+
             CustomMetadataCache.refresh_cache()
-        return TypeDefResponse(**raw_json)
+        elif typedef_type == EnumDef:
+            from pyatlan.cache.enum_cache import EnumCache
 
-    def purge_typedef(self, internal_name: str) -> None:
-        self._call_api(DELETE_TYPE_DEF_BY_NAME.format_path_with_params(internal_name))
-        # TODO: if we know which kind of typedef is being purged, we only need
-        #  to refresh that particular cache
-        from pyatlan.cache.classification_cache import ClassificationCache
-        from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
-        ClassificationCache.refresh_cache()
-        CustomMetadataCache.refresh_cache()
+            EnumCache.refresh_cache()
+        elif typedef_type == ClassificationDef:
+            from pyatlan.cache.classification_cache import ClassificationCache
+
+            ClassificationCache.refresh_cache()
 
     @validate_arguments()
     def add_classifications(
         self,
         asset_type: Type[A],
         qualified_name: str,
         classification_names: list[str],
@@ -621,25 +806,70 @@
     ) -> Optional[A]:
         asset = asset_type()
         asset.qualified_name = qualified_name
         asset.name = name
         asset.remove_announcement()
         return self._update_asset_by_attribute(asset, asset_type, qualified_name)
 
+    def update_custom_metadata_attributes(
+        self, guid: str, custom_metadata: CustomMetadata
+    ):
+        custom_metadata_request = CustomMetadataReqest(__root__=custom_metadata)
+        self._call_api(
+            ADD_BUSINESS_ATTRIBUTE_BY_ID.format_path(
+                {"entity_guid": guid, "bm_id": custom_metadata._meta_data_type_id}
+            ),
+            None,
+            custom_metadata_request,
+        )
+
     def replace_custom_metadata(self, guid: str, custom_metadata: CustomMetadata):
-        # TODO: This endpoint is not currently functioning correctly on the server
+        from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+
+        # Iterate through the custom metadata provided and explicitly set every
+        # single attribute, so that they are all serialized out (forcing removal
+        # of any empty ones)
+        for k, v in custom_metadata.items():
+            # Need to translate the hashed-string key here back to an attribute name
+            attr_name = str(
+                CustomMetadataCache.get_attr_name_for_id(
+                    set_id=custom_metadata._meta_data_type_id, attr_id=k
+                )
+            )
+            if not v:
+                setattr(custom_metadata, attr_name, None)
+            else:
+                setattr(custom_metadata, attr_name, v)
         custom_metadata_request = CustomMetadataReqest(__root__=custom_metadata)
         self._call_api(
             ADD_BUSINESS_ATTRIBUTE_BY_ID.format_path(
                 {"entity_guid": guid, "bm_id": custom_metadata._meta_data_type_id}
             ),
             None,
             custom_metadata_request,
         )
 
+    def remove_custom_metadata(self, guid: str, cm_name: str):
+        from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+
+        # Ensure the custom metadata exists first - let this throw an error if not
+        if cm_id := CustomMetadataCache.get_id_for_name(cm_name):
+            # Initialize a dict of empty attributes for the custom metadata, and then
+            # send that so that they are removed accordingly
+            if cm_type := CustomMetadataCache.get_type_for_id(cm_id):
+                custom_metadata = cm_type()
+                custom_metadata_request = CustomMetadataReqest(__root__=custom_metadata)
+                self._call_api(
+                    ADD_BUSINESS_ATTRIBUTE_BY_ID.format_path(
+                        {"entity_guid": guid, "bm_id": cm_id}
+                    ),
+                    None,
+                    custom_metadata_request,
+                )
+
     @validate_arguments()
     def append_terms(
         self,
         asset_type: Type[A],
         terms: list[AtlasGlossaryTerm],
         guid: Optional[str] = None,
         qualified_name: Optional[str] = None,
```

### Comparing `pyatlan-0.0.31/pyatlan/client/constants.py` & `pyatlan-0.0.32/pyatlan/client/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,25 @@
     BASE_URI,
     MULTIPART_FORM_DATA,
     HTTPMethod,
     HTTPStatus,
 )
 
 ROLE_API = f"{ADMIN_URI}roles"
+GROUP_API = f"{ADMIN_URI}groups"
 
 # Role APIs
 GET_ROLES = API(ROLE_API, HTTPMethod.GET, HTTPStatus.OK)
 
+# Group APIs
+GET_GROUPS = API(GROUP_API, HTTPMethod.GET, HTTPStatus.OK)
+CREATE_GROUP = API(GROUP_API, HTTPMethod.POST, HTTPStatus.OK)
+UPDATE_GROUP = API(GROUP_API, HTTPMethod.POST, HTTPStatus.OK)
+DELETE_GROUP = API(GROUP_API + "/{group_guid}/delete", HTTPMethod.POST, HTTPStatus.OK)
+
 ENTITY_API = f"{BASE_URI}entity/"
 PREFIX_ATTR = "attr:"
 PREFIX_ATTR_ = "attr_"
 ADMIN_API = f"{BASE_URI}admin/"
 ENTITY_PURGE_API = f"{ADMIN_API}purge/"
 ENTITY_BULK_API = f"{ENTITY_API}bulk/"
 BULK_SET_CLASSIFICATIONS = "bulk/setClassifications"
```

### Comparing `pyatlan-0.0.31/pyatlan/error.py` & `pyatlan-0.0.32/pyatlan/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     def __init__(
         self,
         message: str,
         code: str,
         status_code: Optional[int] = None,
         should_retry: bool = False,
     ):
-
         super(APIConnectionError, self).__init__(message, code, status_code)
         self.should_retry = should_retry
 
 
 class AtlanErrorWithParamCode(AtlanError):
     def __init__(self, message: str, param: str, code: str, status_code: int):
         self.param = param
```

### Comparing `pyatlan-0.0.31/pyatlan/exceptions.py` & `pyatlan-0.0.32/pyatlan/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     def __init__(
         self,
         message: str,
         status_code: int,
         code: Optional[str],
         cause: Optional[Exception] = None,
     ):
+        super().__init__(message)
         self.message = message
         self.code = code
         self.status_code = status_code
         self.cause = cause
 
 
 class InvalidRequestException(AtlanException):
```

### Comparing `pyatlan-0.0.31/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.0.32/pyatlan/generator/generate_from_typdefs.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ]
 ARRAY_REPLACEMENTS = [("array<string>", "set{string}")]
 
 
 def get_type(type_: str):
     ret_value = type_
 
-    for (field, replacement) in TYPE_REPLACEMENTS:
+    for field, replacement in TYPE_REPLACEMENTS:
         ret_value = ret_value.replace(field, replacement)
     return ret_value
 
 
 def to_dict(entity_defs: list[EntityDef]) -> dict[str, EntityDef]:
     return {entity_def.name: entity_def for entity_def in entity_defs}
```

### Comparing `pyatlan-0.0.31/pyatlan/model/assets.py` & `pyatlan-0.0.32/pyatlan/model/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,17 +53,20 @@
     BadgeCondition,
     ColumnValueFrequencyMap,
     DbtMetricFilter,
     GoogleLabel,
     GoogleTag,
     Histogram,
     KafkaTopicConsumption,
+    MCRuleComparison,
+    MCRuleSchedule,
     PopularityInsights,
+    SourceTagAttribute,
 )
-from pyatlan.utils import next_id
+from pyatlan.utils import next_id, validate_required_fields
 
 
 def validate_single_required_field(field_names: list[str], values: list[Any]):
     indexes = [idx for idx, value in enumerate(values) if value is not None]
     if not indexes:
         raise ValueError(
             f"One of the following parameters are required: {', '.join(field_names)}"
@@ -71,24 +74,14 @@
     if len(indexes) > 1:
         names = [field_names[idx] for idx in indexes]
         raise ValueError(
             f"Only one of the following parameters are allowed: {', '.join(names)}"
         )
 
 
-def validate_required_fields(field_names: list[str], values: list[Any]):
-    for field_name, value in zip(field_names, values):
-        if value is None:
-            raise ValueError(f"{field_name} is required")
-        if isinstance(value, str) and not value.strip():
-            raise ValueError(f"{field_name} cannot be blank")
-        if isinstance(value, list) and len(value) == 0:
-            raise ValueError(f"{field_name} cannot be an empty list")
-
-
 SelfAsset = TypeVar("SelfAsset", bound="Asset")
 
 
 class Referenceable(AtlanObject):
     """Description"""
 
     def __init__(__pydantic_self__, **data: Any) -> None:
@@ -413,14 +406,26 @@
         "asset_dbt_environment_name",
         "asset_dbt_environment_dbt_version",
         "asset_dbt_tags",
         "asset_dbt_semantic_layer_proxy_url",
         "asset_dbt_source_freshness_criteria",
         "sample_data_url",
         "asset_tags",
+        "asset_mc_incident_names",
+        "asset_mc_incident_qualified_names",
+        "asset_mc_monitor_names",
+        "asset_mc_monitor_qualified_names",
+        "asset_mc_monitor_statuses",
+        "asset_mc_monitor_types",
+        "asset_mc_monitor_schedule_types",
+        "asset_mc_incident_types",
+        "asset_mc_incident_sub_types",
+        "asset_mc_incident_severities",
+        "asset_mc_incident_states",
+        "asset_mc_last_sync_run_at",
         "terms",
     ]
 
     @property
     def name(self) -> str:
         return self.attributes.name
 
@@ -1520,14 +1525,150 @@
     @asset_tags.setter
     def asset_tags(self, asset_tags: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_tags = asset_tags
 
     @property
+    def asset_mc_incident_names(self) -> Optional[set[str]]:
+        return self.attributes.asset_mc_incident_names
+
+    @asset_mc_incident_names.setter
+    def asset_mc_incident_names(self, asset_mc_incident_names: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_incident_names = asset_mc_incident_names
+
+    @property
+    def asset_mc_incident_qualified_names(self) -> Optional[set[str]]:
+        return self.attributes.asset_mc_incident_qualified_names
+
+    @asset_mc_incident_qualified_names.setter
+    def asset_mc_incident_qualified_names(
+        self, asset_mc_incident_qualified_names: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_incident_qualified_names = (
+            asset_mc_incident_qualified_names
+        )
+
+    @property
+    def asset_mc_monitor_names(self) -> Optional[set[str]]:
+        return self.attributes.asset_mc_monitor_names
+
+    @asset_mc_monitor_names.setter
+    def asset_mc_monitor_names(self, asset_mc_monitor_names: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_monitor_names = asset_mc_monitor_names
+
+    @property
+    def asset_mc_monitor_qualified_names(self) -> Optional[set[str]]:
+        return self.attributes.asset_mc_monitor_qualified_names
+
+    @asset_mc_monitor_qualified_names.setter
+    def asset_mc_monitor_qualified_names(
+        self, asset_mc_monitor_qualified_names: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_monitor_qualified_names = (
+            asset_mc_monitor_qualified_names
+        )
+
+    @property
+    def asset_mc_monitor_statuses(self) -> Optional[set[str]]:
+        return self.attributes.asset_mc_monitor_statuses
+
+    @asset_mc_monitor_statuses.setter
+    def asset_mc_monitor_statuses(self, asset_mc_monitor_statuses: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_monitor_statuses = asset_mc_monitor_statuses
+
+    @property
+    def asset_mc_monitor_types(self) -> Optional[set[str]]:
+        return self.attributes.asset_mc_monitor_types
+
+    @asset_mc_monitor_types.setter
+    def asset_mc_monitor_types(self, asset_mc_monitor_types: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_monitor_types = asset_mc_monitor_types
+
+    @property
+    def asset_mc_monitor_schedule_types(self) -> Optional[set[str]]:
+        return self.attributes.asset_mc_monitor_schedule_types
+
+    @asset_mc_monitor_schedule_types.setter
+    def asset_mc_monitor_schedule_types(
+        self, asset_mc_monitor_schedule_types: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_monitor_schedule_types = (
+            asset_mc_monitor_schedule_types
+        )
+
+    @property
+    def asset_mc_incident_types(self) -> Optional[set[str]]:
+        return self.attributes.asset_mc_incident_types
+
+    @asset_mc_incident_types.setter
+    def asset_mc_incident_types(self, asset_mc_incident_types: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_incident_types = asset_mc_incident_types
+
+    @property
+    def asset_mc_incident_sub_types(self) -> Optional[set[str]]:
+        return self.attributes.asset_mc_incident_sub_types
+
+    @asset_mc_incident_sub_types.setter
+    def asset_mc_incident_sub_types(
+        self, asset_mc_incident_sub_types: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_incident_sub_types = asset_mc_incident_sub_types
+
+    @property
+    def asset_mc_incident_severities(self) -> Optional[set[str]]:
+        return self.attributes.asset_mc_incident_severities
+
+    @asset_mc_incident_severities.setter
+    def asset_mc_incident_severities(
+        self, asset_mc_incident_severities: Optional[set[str]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_incident_severities = asset_mc_incident_severities
+
+    @property
+    def asset_mc_incident_states(self) -> Optional[set[str]]:
+        return self.attributes.asset_mc_incident_states
+
+    @asset_mc_incident_states.setter
+    def asset_mc_incident_states(self, asset_mc_incident_states: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_incident_states = asset_mc_incident_states
+
+    @property
+    def asset_mc_last_sync_run_at(self) -> Optional[datetime]:
+        return self.attributes.asset_mc_last_sync_run_at
+
+    @asset_mc_last_sync_run_at.setter
+    def asset_mc_last_sync_run_at(self, asset_mc_last_sync_run_at: Optional[datetime]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_mc_last_sync_run_at = asset_mc_last_sync_run_at
+
+    @property
     def terms(self) -> list[AtlasGlossaryTerm]:
         if self.attributes is None:
             self.attributes = self.Attributes()
         return [] if self.attributes.meanings is None else self.attributes.meanings
 
     @terms.setter
     def terms(self, terms: list[AtlasGlossaryTerm]):
@@ -1566,15 +1707,14 @@
 
     @classmethod
     def __get_validators__(cls):
         yield cls._convert_to_real_type_
 
     @classmethod
     def _convert_to_real_type_(cls, data):
-
         if isinstance(data, Asset):
             return data
 
         data_type = (
             data.get("type_name") if "type_name" in data else data.get("typeName")
         )
 
@@ -1864,14 +2004,56 @@
         asset_dbt_source_freshness_criteria: Optional[str] = Field(
             None, description="", alias="assetDbtSourceFreshnessCriteria"
         )
         sample_data_url: Optional[str] = Field(
             None, description="", alias="sampleDataUrl"
         )
         asset_tags: Optional[set[str]] = Field(None, description="", alias="assetTags")
+        asset_mc_incident_names: Optional[set[str]] = Field(
+            None, description="", alias="assetMcIncidentNames"
+        )
+        asset_mc_incident_qualified_names: Optional[set[str]] = Field(
+            None, description="", alias="assetMcIncidentQualifiedNames"
+        )
+        asset_mc_monitor_names: Optional[set[str]] = Field(
+            None, description="", alias="assetMcMonitorNames"
+        )
+        asset_mc_monitor_qualified_names: Optional[set[str]] = Field(
+            None, description="", alias="assetMcMonitorQualifiedNames"
+        )
+        asset_mc_monitor_statuses: Optional[set[str]] = Field(
+            None, description="", alias="assetMcMonitorStatuses"
+        )
+        asset_mc_monitor_types: Optional[set[str]] = Field(
+            None, description="", alias="assetMcMonitorTypes"
+        )
+        asset_mc_monitor_schedule_types: Optional[set[str]] = Field(
+            None, description="", alias="assetMcMonitorScheduleTypes"
+        )
+        asset_mc_incident_types: Optional[set[str]] = Field(
+            None, description="", alias="assetMcIncidentTypes"
+        )
+        asset_mc_incident_sub_types: Optional[set[str]] = Field(
+            None, description="", alias="assetMcIncidentSubTypes"
+        )
+        asset_mc_incident_severities: Optional[set[str]] = Field(
+            None, description="", alias="assetMcIncidentSeverities"
+        )
+        asset_mc_incident_states: Optional[set[str]] = Field(
+            None, description="", alias="assetMcIncidentStates"
+        )
+        asset_mc_last_sync_run_at: Optional[datetime] = Field(
+            None, description="", alias="assetMcLastSyncRunAt"
+        )
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -2041,17 +2223,23 @@
             None, description="", alias="longDescription"
         )
         language: Optional[str] = Field(None, description="", alias="language")
         usage: Optional[str] = Field(None, description="", alias="usage")
         additional_attributes: Optional[dict[str, str]] = Field(
             None, description="", alias="additionalAttributes"
         )
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         terms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="terms"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         categories: Optional[list[AtlasGlossaryCategory]] = Field(
             None, description="", alias="categories"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -2122,14 +2310,20 @@
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "DataSet":
             raise ValueError("must be DataSet")
         return v
 
     class Attributes(Asset.Attributes):
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -2175,14 +2369,20 @@
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "ProcessExecution":
             raise ValueError("must be ProcessExecution")
         return v
 
     class Attributes(Asset.Attributes):
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -2333,14 +2533,17 @@
         )  # relationship
         meanings: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="meanings"
         )  # relationship
         see_also: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="seeAlso"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         translated_terms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="translatedTerms"
         )  # relationship
         is_a: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="isA"
         )  # relationship
         anchor: AtlasGlossary = Field(
@@ -2348,14 +2551,17 @@
         )  # relationship
         antonyms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="antonyms"
         )  # relationship
         assigned_entities: Optional[list[Referenceable]] = Field(
             None, description="", alias="assignedEntities"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         classifies: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="classifies"
         )  # relationship
         categories: Optional[list[AtlasGlossaryCategory]] = Field(
@@ -2487,14 +2693,20 @@
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Cloud":
             raise ValueError("must be Cloud")
         return v
 
     class Attributes(Asset.Attributes):
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -2540,14 +2752,20 @@
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Infrastructure":
             raise ValueError("must be Infrastructure")
         return v
 
     class Attributes(Asset.Attributes):
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -2879,14 +3097,20 @@
         )
         has_popularity_insights: Optional[bool] = Field(
             None, description="", alias="hasPopularityInsights"
         )
         connection_dbt_environments: Optional[set[str]] = Field(
             None, description="", alias="connectionDbtEnvironments"
         )
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -3065,14 +3289,20 @@
 
     class Attributes(Asset.Attributes):
         inputs: Optional[list[Catalog]] = Field(None, description="", alias="inputs")
         outputs: Optional[list[Catalog]] = Field(None, description="", alias="outputs")
         code: Optional[str] = Field(None, description="", alias="code")
         sql: Optional[str] = Field(None, description="", alias="sql")
         ast: Optional[str] = Field(None, description="", alias="ast")
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -3248,23 +3478,29 @@
         )
         long_description: Optional[str] = Field(
             None, description="", alias="longDescription"
         )
         additional_attributes: Optional[dict[str, str]] = Field(
             None, description="", alias="additionalAttributes"
         )
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         terms: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="terms"
         )  # relationship
         anchor: AtlasGlossary = Field(
             None, description="", alias="anchor"
         )  # relationship
         parent_category: Optional[AtlasGlossaryCategory] = Field(
             None, description="", alias="parentCategory"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         children_categories: Optional[list[AtlasGlossaryCategory]] = Field(
             None, description="", alias="childrenCategories"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -3377,34 +3613,86 @@
 
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Badge":
             raise ValueError("must be Badge")
         return v
 
+    @classmethod
+    # @validate_arguments()
+    def create(
+        cls,
+        *,
+        name: StrictStr,
+        cm_name: str,
+        cm_attribute: str,
+        badge_conditions: list[BadgeCondition],
+    ) -> Badge:
+        return cls(
+            attributes=Badge.Attributes.create(
+                name=name,
+                cm_name=cm_name,
+                cm_attribute=cm_attribute,
+                badge_conditions=badge_conditions,
+            )
+        )
+
     class Attributes(Asset.Attributes):
         badge_conditions: Optional[list[BadgeCondition]] = Field(
             None, description="", alias="badgeConditions"
         )
         badge_metadata_attribute: Optional[str] = Field(
             None, description="", alias="badgeMetadataAttribute"
         )
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
             None, description="", alias="readme"
         )  # relationship
         meanings: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="meanings"
         )  # relationship
 
+        @classmethod
+        # @validate_arguments()
+        def create(
+            cls,
+            *,
+            name: StrictStr,
+            cm_name: str,
+            cm_attribute: str,
+            badge_conditions: list[BadgeCondition],
+        ) -> Badge.Attributes:
+            validate_required_fields(
+                ["name", "cm_name", "cm_attribute", "badge_conditions"],
+                [name, cm_name, cm_attribute, badge_conditions],
+            )
+            from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+
+            cm_id = CustomMetadataCache.get_id_for_name(cm_name)
+            cm_attr_id = CustomMetadataCache.get_attr_id_for_name(
+                set_name=cm_name, attr_name=cm_attribute
+            )
+            return Badge.Attributes(
+                name=name,
+                qualified_name=f"badges/global/{cm_id}.{cm_attr_id}",
+                badge_metadata_attribute=f"{cm_id}.{cm_attr_id}",
+                badge_conditions=badge_conditions,
+            )
+
     attributes: "Badge.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
@@ -3437,17 +3725,23 @@
     @validator("type_name")
     def validate_type_name(cls, v):
         if v != "Namespace":
             raise ValueError("must be Namespace")
         return v
 
     class Attributes(Asset.Attributes):
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         children_queries: Optional[list[Query]] = Field(
             None, description="", alias="childrenQueries"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         children_folders: Optional[list[Folder]] = Field(
             None, description="", alias="childrenFolders"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -3499,14 +3793,20 @@
             raise ValueError("must be Catalog")
         return v
 
     class Attributes(Asset.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -3667,14 +3967,20 @@
         )
         google_labels: Optional[list[GoogleLabel]] = Field(
             None, description="", alias="googleLabels"
         )
         google_tags: Optional[list[GoogleTag]] = Field(
             None, description="", alias="googleTags"
         )
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -3780,14 +4086,20 @@
         )
         adls_account_secondary_location: Optional[str] = Field(
             None, description="", alias="adlsAccountSecondaryLocation"
         )
         azure_tags: Optional[list[AzureTag]] = Field(
             None, description="", alias="azureTags"
         )
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -3947,14 +4259,20 @@
             None, description="", alias="awsResourceId"
         )
         aws_owner_name: Optional[str] = Field(
             None, description="", alias="awsOwnerName"
         )
         aws_owner_id: Optional[str] = Field(None, description="", alias="awsOwnerId")
         aws_tags: Optional[list[AwsTag]] = Field(None, description="", alias="awsTags")
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -4003,17 +4321,23 @@
             raise ValueError("must be BIProcess")
         return v
 
     class Attributes(Process.Attributes):
         outputs: Optional[list[Catalog]] = Field(
             None, description="", alias="outputs"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         inputs: Optional[list[Catalog]] = Field(
             None, description="", alias="inputs"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -4068,17 +4392,23 @@
     class Attributes(Process.Attributes):
         outputs: Optional[list[Catalog]] = Field(
             None, description="", alias="outputs"
         )  # relationship
         process: Optional[Process] = Field(
             None, description="", alias="process"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         inputs: Optional[list[Catalog]] = Field(
             None, description="", alias="inputs"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -4151,17 +4481,23 @@
         if v != "Collection":
             raise ValueError("must be Collection")
         return v
 
     class Attributes(Namespace.Attributes):
         icon: Optional[str] = Field(None, description="", alias="icon")
         icon_type: Optional[IconType] = Field(None, description="", alias="iconType")
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         children_queries: Optional[list[Query]] = Field(
             None, description="", alias="childrenQueries"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -4239,17 +4575,23 @@
         parent_qualified_name: str = Field(
             None, description="", alias="parentQualifiedName"
         )
         collection_qualified_name: str = Field(
             None, description="", alias="collectionQualifiedName"
         )
         parent: Namespace = Field(None, description="", alias="parent")  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         children_queries: Optional[list[Query]] = Field(
             None, description="", alias="childrenQueries"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -4301,14 +4643,20 @@
             raise ValueError("must be EventStore")
         return v
 
     class Attributes(Catalog.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -4360,14 +4708,20 @@
             raise ValueError("must be ObjectStore")
         return v
 
     class Attributes(Catalog.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -4419,14 +4773,20 @@
             raise ValueError("must be DataQuality")
         return v
 
     class Attributes(Catalog.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -4478,14 +4838,20 @@
             raise ValueError("must be BI")
         return v
 
     class Attributes(Catalog.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -4537,14 +4903,20 @@
             raise ValueError("must be SaaS")
         return v
 
     class Attributes(Catalog.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -4842,14 +5214,20 @@
         )
         dbt_semantic_layer_proxy_url: Optional[str] = Field(
             None, description="", alias="dbtSemanticLayerProxyUrl"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -4951,14 +5329,20 @@
         reference: Optional[str] = Field(None, description="", alias="reference")
         resource_metadata: Optional[dict[str, str]] = Field(
             None, description="", alias="resourceMetadata"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -5010,14 +5394,20 @@
             raise ValueError("must be Insight")
         return v
 
     class Attributes(Catalog.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -5149,14 +5539,20 @@
         )
         api_is_auth_optional: Optional[bool] = Field(
             None, description="", alias="apiIsAuthOptional"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -5172,14 +5568,133 @@
     attributes: "API.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class Tag(Catalog):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in Tag._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "tag_id",
+        "tag_attributes",
+        "tag_allowed_values",
+        "mapped_classification_name",
+        "terms",
+    ]
+
+    @property
+    def tag_id(self) -> Optional[str]:
+        return self.attributes.tag_id
+
+    @tag_id.setter
+    def tag_id(self, tag_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tag_id = tag_id
+
+    @property
+    def tag_attributes(self) -> Optional[list[SourceTagAttribute]]:
+        return self.attributes.tag_attributes
+
+    @tag_attributes.setter
+    def tag_attributes(self, tag_attributes: Optional[list[SourceTagAttribute]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tag_attributes = tag_attributes
+
+    @property
+    def tag_allowed_values(self) -> Optional[set[str]]:
+        return self.attributes.tag_allowed_values
+
+    @tag_allowed_values.setter
+    def tag_allowed_values(self, tag_allowed_values: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tag_allowed_values = tag_allowed_values
+
+    @property
+    def mapped_classification_name(self) -> Optional[str]:
+        return self.attributes.mapped_classification_name
+
+    @mapped_classification_name.setter
+    def mapped_classification_name(self, mapped_classification_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mapped_classification_name = mapped_classification_name
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
+    type_name: str = Field("Tag", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "Tag":
+            raise ValueError("must be Tag")
+        return v
+
+    class Attributes(Catalog.Attributes):
+        tag_id: Optional[str] = Field(None, description="", alias="tagId")
+        tag_attributes: Optional[list[SourceTagAttribute]] = Field(
+            None, description="", alias="tagAttributes"
+        )
+        tag_allowed_values: Optional[set[str]] = Field(
+            None, description="", alias="tagAllowedValues"
+        )
+        mapped_classification_name: Optional[str] = Field(
+            None, description="", alias="mappedClassificationName"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "Tag.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class SQL(Catalog):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in SQL._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -5398,14 +5913,20 @@
         )  # relationship
         dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="dbtModels"
         )  # relationship
         dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="dbtSources"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -5575,14 +6096,20 @@
         )
         google_tags: Optional[list[GoogleTag]] = Field(
             None, description="", alias="googleTags"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -5828,14 +6355,20 @@
         )
         google_tags: Optional[list[GoogleTag]] = Field(
             None, description="", alias="googleTags"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -6059,14 +6592,20 @@
         )
         google_tags: Optional[list[GoogleTag]] = Field(
             None, description="", alias="googleTags"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -6192,14 +6731,20 @@
         )
         azure_tags: Optional[list[AzureTag]] = Field(
             None, description="", alias="azureTags"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -6389,14 +6934,20 @@
             None, description="", alias="awsOwnerName"
         )
         aws_owner_id: Optional[str] = Field(None, description="", alias="awsOwnerId")
         aws_tags: Optional[list[AwsTag]] = Field(None, description="", alias="awsTags")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -6770,17 +7321,23 @@
         outputs: Optional[list[Catalog]] = Field(None, description="", alias="outputs")
         code: Optional[str] = Field(None, description="", alias="code")
         sql: Optional[str] = Field(None, description="", alias="sql")
         ast: Optional[str] = Field(None, description="", alias="ast")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         process: Optional[Process] = Field(
             None, description="", alias="process"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -6835,14 +7392,20 @@
             raise ValueError("must be Kafka")
         return v
 
     class Attributes(EventStore.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -6858,14 +7421,105 @@
     attributes: "Kafka.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class MonteCarlo(DataQuality):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MonteCarlo._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "mc_labels",
+        "mc_asset_qualified_names",
+        "terms",
+    ]
+
+    @property
+    def mc_labels(self) -> Optional[set[str]]:
+        return self.attributes.mc_labels
+
+    @mc_labels.setter
+    def mc_labels(self, mc_labels: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_labels = mc_labels
+
+    @property
+    def mc_asset_qualified_names(self) -> Optional[set[str]]:
+        return self.attributes.mc_asset_qualified_names
+
+    @mc_asset_qualified_names.setter
+    def mc_asset_qualified_names(self, mc_asset_qualified_names: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_asset_qualified_names = mc_asset_qualified_names
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
+    type_name: str = Field("MonteCarlo", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MonteCarlo":
+            raise ValueError("must be MonteCarlo")
+        return v
+
+    class Attributes(DataQuality.Attributes):
+        mc_labels: Optional[set[str]] = Field(None, description="", alias="mcLabels")
+        mc_asset_qualified_names: Optional[set[str]] = Field(
+            None, description="", alias="mcAssetQualifiedNames"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "MonteCarlo.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class Metric(DataQuality):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Metric._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -6946,23 +7600,29 @@
         )
         metric_time_grains: Optional[set[str]] = Field(
             None, description="", alias="metricTimeGrains"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         assets: Optional[list[Asset]] = Field(
             None, description="", alias="assets"
         )  # relationship
         metric_dimension_columns: Optional[list[Column]] = Field(
             None, description="", alias="metricDimensionColumns"
         )  # relationship
         metric_timestamp_column: Optional[Column] = Field(
             None, description="", alias="metricTimestampColumn"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -7046,14 +7706,20 @@
         )
         metabase_collection_qualified_name: Optional[str] = Field(
             None, description="", alias="metabaseCollectionQualifiedName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -7147,14 +7813,20 @@
         )
         quick_sight_sheet_name: Optional[str] = Field(
             None, description="", alias="quickSightSheetName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -7234,14 +7906,20 @@
         )
         thoughtspot_question_text: Optional[str] = Field(
             None, description="", alias="thoughtspotQuestionText"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -7353,14 +8031,20 @@
         )
         power_b_i_endorsement: Optional[PowerbiEndorsement] = Field(
             None, description="", alias="powerBIEndorsement"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -7476,14 +8160,20 @@
         )
         preset_dashboard_qualified_name: Optional[str] = Field(
             None, description="", alias="presetDashboardQualifiedName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -7659,14 +8349,20 @@
         )
         mode_query_qualified_name: Optional[str] = Field(
             None, description="", alias="modeQueryQualifiedName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -7808,14 +8504,20 @@
         )
         sigma_data_element_name: Optional[str] = Field(
             None, description="", alias="sigmaDataElementName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -7969,14 +8671,20 @@
         qlik_owner_id: Optional[str] = Field(None, description="", alias="qlikOwnerId")
         qlik_is_published: Optional[bool] = Field(
             None, description="", alias="qlikIsPublished"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -8028,14 +8736,20 @@
             raise ValueError("must be Tableau")
         return v
 
     class Attributes(BI.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -8087,14 +8801,20 @@
             raise ValueError("must be Looker")
         return v
 
     class Attributes(BI.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -8160,14 +8880,20 @@
     class Attributes(BI.Attributes):
         redash_is_published: Optional[bool] = Field(
             None, description="", alias="redashIsPublished"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -8245,14 +8971,20 @@
         organization_qualified_name: Optional[str] = Field(
             None, description="", alias="organizationQualifiedName"
         )
         api_name: Optional[str] = Field(None, description="", alias="apiName")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -8349,20 +9081,26 @@
         )
         dbt_model_column_sql_columns: Optional[list[Column]] = Field(
             None, description="", alias="dbtModelColumnSqlColumns"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         sql_column: Optional[Column] = Field(
             None, description="", alias="sqlColumn"
         )  # relationship
         dbt_model: Optional[DbtModel] = Field(
             None, description="", alias="dbtModel"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -8601,17 +9339,23 @@
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         dbt_metrics: Optional[list[DbtMetric]] = Field(
             None, description="", alias="dbtMetrics"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         dbt_model_sql_assets: Optional[list[SQL]] = Field(
             None, description="", alias="dbtModelSqlAssets"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -8981,41 +9725,47 @@
         )
         metric_time_grains: Optional[set[str]] = Field(
             None, description="", alias="metricTimeGrains"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        metric_timestamp_column: Optional[Column] = Field(
+            None, description="", alias="metricTimestampColumn"
+        )  # relationship
+        dbt_model: Optional[DbtModel] = Field(
+            None, description="", alias="dbtModel"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         assets: Optional[list[Asset]] = Field(
             None, description="", alias="assets"
         )  # relationship
         metric_dimension_columns: Optional[list[Column]] = Field(
             None, description="", alias="metricDimensionColumns"
         )  # relationship
-        metric_timestamp_column: Optional[Column] = Field(
-            None, description="", alias="metricTimestampColumn"
-        )  # relationship
         dbt_metric_filter_columns: Optional[list[Column]] = Field(
             None, description="", alias="dbtMetricFilterColumns"
         )  # relationship
-        dbt_model: Optional[DbtModel] = Field(
-            None, description="", alias="dbtModel"
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
     attributes: "DbtMetric.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
@@ -9081,17 +9831,23 @@
         dbt_state: Optional[str] = Field(None, description="", alias="dbtState")
         dbt_freshness_criteria: Optional[str] = Field(
             None, description="", alias="dbtFreshnessCriteria"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         sql_assets: Optional[list[SQL]] = Field(
             None, description="", alias="sqlAssets"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -9466,14 +10222,20 @@
         outputs: Optional[list[Catalog]] = Field(None, description="", alias="outputs")
         code: Optional[str] = Field(None, description="", alias="code")
         sql: Optional[str] = Field(None, description="", alias="sql")
         ast: Optional[str] = Field(None, description="", alias="ast")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -9552,14 +10314,20 @@
 
     class Attributes(Resource.Attributes):
         icon: Optional[str] = Field(None, description="", alias="icon")
         icon_type: Optional[IconType] = Field(None, description="", alias="iconType")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -9635,17 +10403,23 @@
             quote(description) if description is not None else description
         )
 
     class Attributes(Resource.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         internal: Optional[Internal] = Field(
             None, description="", alias="__internal"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -9754,14 +10528,20 @@
         icon_type: Optional[IconType] = Field(None, description="", alias="iconType")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         internal: Optional[Internal] = Field(
             None, description="", alias="internal"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -9930,17 +10710,23 @@
         )
         api_spec_service_alias: Optional[str] = Field(
             None, description="", alias="apiSpecServiceAlias"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         api_paths: Optional[list[APIPath]] = Field(
             None, description="", alias="apiPaths"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -10082,14 +10868,20 @@
         )
         api_path_is_ingress_exposed: Optional[bool] = Field(
             None, description="", alias="apiPathIsIngressExposed"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -10108,14 +10900,332 @@
     attributes: "APIPath.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class SnowflakeTag(Tag):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in SnowflakeTag._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "tag_id",
+        "tag_attributes",
+        "tag_allowed_values",
+        "mapped_classification_name",
+        "query_count",
+        "query_user_count",
+        "query_user_map",
+        "query_count_updated_at",
+        "database_name",
+        "database_qualified_name",
+        "schema_name",
+        "schema_qualified_name",
+        "table_name",
+        "table_qualified_name",
+        "view_name",
+        "view_qualified_name",
+        "is_profiled",
+        "last_profiled_at",
+        "terms",
+    ]
+
+    @property
+    def tag_id(self) -> Optional[str]:
+        return self.attributes.tag_id
+
+    @tag_id.setter
+    def tag_id(self, tag_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tag_id = tag_id
+
+    @property
+    def tag_attributes(self) -> Optional[list[SourceTagAttribute]]:
+        return self.attributes.tag_attributes
+
+    @tag_attributes.setter
+    def tag_attributes(self, tag_attributes: Optional[list[SourceTagAttribute]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tag_attributes = tag_attributes
+
+    @property
+    def tag_allowed_values(self) -> Optional[set[str]]:
+        return self.attributes.tag_allowed_values
+
+    @tag_allowed_values.setter
+    def tag_allowed_values(self, tag_allowed_values: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.tag_allowed_values = tag_allowed_values
+
+    @property
+    def mapped_classification_name(self) -> Optional[str]:
+        return self.attributes.mapped_classification_name
+
+    @mapped_classification_name.setter
+    def mapped_classification_name(self, mapped_classification_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mapped_classification_name = mapped_classification_name
+
+    @property
+    def query_count(self) -> Optional[int]:
+        return self.attributes.query_count
+
+    @query_count.setter
+    def query_count(self, query_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.query_count = query_count
+
+    @property
+    def query_user_count(self) -> Optional[int]:
+        return self.attributes.query_user_count
+
+    @query_user_count.setter
+    def query_user_count(self, query_user_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.query_user_count = query_user_count
+
+    @property
+    def query_user_map(self) -> Optional[dict[str, int]]:
+        return self.attributes.query_user_map
+
+    @query_user_map.setter
+    def query_user_map(self, query_user_map: Optional[dict[str, int]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.query_user_map = query_user_map
+
+    @property
+    def query_count_updated_at(self) -> Optional[datetime]:
+        return self.attributes.query_count_updated_at
+
+    @query_count_updated_at.setter
+    def query_count_updated_at(self, query_count_updated_at: Optional[datetime]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.query_count_updated_at = query_count_updated_at
+
+    @property
+    def database_name(self) -> Optional[str]:
+        return self.attributes.database_name
+
+    @database_name.setter
+    def database_name(self, database_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.database_name = database_name
+
+    @property
+    def database_qualified_name(self) -> Optional[str]:
+        return self.attributes.database_qualified_name
+
+    @database_qualified_name.setter
+    def database_qualified_name(self, database_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.database_qualified_name = database_qualified_name
+
+    @property
+    def schema_name(self) -> Optional[str]:
+        return self.attributes.schema_name
+
+    @schema_name.setter
+    def schema_name(self, schema_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.schema_name = schema_name
+
+    @property
+    def schema_qualified_name(self) -> Optional[str]:
+        return self.attributes.schema_qualified_name
+
+    @schema_qualified_name.setter
+    def schema_qualified_name(self, schema_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.schema_qualified_name = schema_qualified_name
+
+    @property
+    def table_name(self) -> Optional[str]:
+        return self.attributes.table_name
+
+    @table_name.setter
+    def table_name(self, table_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.table_name = table_name
+
+    @property
+    def table_qualified_name(self) -> Optional[str]:
+        return self.attributes.table_qualified_name
+
+    @table_qualified_name.setter
+    def table_qualified_name(self, table_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.table_qualified_name = table_qualified_name
+
+    @property
+    def view_name(self) -> Optional[str]:
+        return self.attributes.view_name
+
+    @view_name.setter
+    def view_name(self, view_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.view_name = view_name
+
+    @property
+    def view_qualified_name(self) -> Optional[str]:
+        return self.attributes.view_qualified_name
+
+    @view_qualified_name.setter
+    def view_qualified_name(self, view_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.view_qualified_name = view_qualified_name
+
+    @property
+    def is_profiled(self) -> Optional[bool]:
+        return self.attributes.is_profiled
+
+    @is_profiled.setter
+    def is_profiled(self, is_profiled: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.is_profiled = is_profiled
+
+    @property
+    def last_profiled_at(self) -> Optional[datetime]:
+        return self.attributes.last_profiled_at
+
+    @last_profiled_at.setter
+    def last_profiled_at(self, last_profiled_at: Optional[datetime]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.last_profiled_at = last_profiled_at
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
+    type_name: str = Field("SnowflakeTag", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "SnowflakeTag":
+            raise ValueError("must be SnowflakeTag")
+        return v
+
+    class Attributes(Tag.Attributes):
+        tag_id: Optional[str] = Field(None, description="", alias="tagId")
+        tag_attributes: Optional[list[SourceTagAttribute]] = Field(
+            None, description="", alias="tagAttributes"
+        )
+        tag_allowed_values: Optional[set[str]] = Field(
+            None, description="", alias="tagAllowedValues"
+        )
+        mapped_classification_name: Optional[str] = Field(
+            None, description="", alias="mappedClassificationName"
+        )
+        query_count: Optional[int] = Field(None, description="", alias="queryCount")
+        query_user_count: Optional[int] = Field(
+            None, description="", alias="queryUserCount"
+        )
+        query_user_map: Optional[dict[str, int]] = Field(
+            None, description="", alias="queryUserMap"
+        )
+        query_count_updated_at: Optional[datetime] = Field(
+            None, description="", alias="queryCountUpdatedAt"
+        )
+        database_name: Optional[str] = Field(None, description="", alias="databaseName")
+        database_qualified_name: Optional[str] = Field(
+            None, description="", alias="databaseQualifiedName"
+        )
+        schema_name: Optional[str] = Field(None, description="", alias="schemaName")
+        schema_qualified_name: Optional[str] = Field(
+            None, description="", alias="schemaQualifiedName"
+        )
+        table_name: Optional[str] = Field(None, description="", alias="tableName")
+        table_qualified_name: Optional[str] = Field(
+            None, description="", alias="tableQualifiedName"
+        )
+        view_name: Optional[str] = Field(None, description="", alias="viewName")
+        view_qualified_name: Optional[str] = Field(
+            None, description="", alias="viewQualifiedName"
+        )
+        is_profiled: Optional[bool] = Field(None, description="", alias="isProfiled")
+        last_profiled_at: Optional[datetime] = Field(
+            None, description="", alias="lastProfiledAt"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        dbt_sources: Optional[list[DbtSource]] = Field(
+            None, description="", alias="dbtSources"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        sql_dbt_models: Optional[list[DbtModel]] = Field(
+            None, description="", alias="sqlDbtModels"
+        )  # relationship
+        sql_dbt_sources: Optional[list[DbtSource]] = Field(
+            None, description="", alias="sqlDBTSources"
+        )  # relationship
+        dbt_models: Optional[list[DbtModel]] = Field(
+            None, description="", alias="dbtModels"
+        )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        atlan_schema: Optional[Schema] = Field(
+            None, description="", alias="atlanSchema"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "SnowflakeTag.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class TablePartition(SQL):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in TablePartition._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -10342,47 +11452,53 @@
         )
         partition_list: Optional[str] = Field(
             None, description="", alias="partitionList"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
         dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="dbtSources"
         )  # relationship
         columns: Optional[list[Column]] = Field(
             None, description="", alias="columns"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        parent_table: Optional[Table] = Field(
-            None, description="", alias="parentTable"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
         readme: Optional[Readme] = Field(
             None, description="", alias="readme"
         )  # relationship
         meanings: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="meanings"
         )  # relationship
         sql_dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="sqlDbtModels"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
         sql_dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="sqlDBTSources"
         )  # relationship
+        dbt_models: Optional[list[DbtModel]] = Field(
+            None, description="", alias="dbtModels"
+        )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        parent_table: Optional[Table] = Field(
+            None, description="", alias="parentTable"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
 
     attributes: "TablePartition.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
@@ -10632,17 +11748,23 @@
         )  # relationship
         sql_dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="sqlDBTSources"
         )  # relationship
         dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="dbtModels"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
@@ -10891,14 +12013,20 @@
         )  # relationship
         dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="dbtModels"
         )  # relationship
         tables: Optional[list[Table]] = Field(
             None, description="", alias="tables"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         views: Optional[list[View]] = Field(
@@ -11598,14 +12726,20 @@
         dbt_metrics: Optional[list[DbtMetric]] = Field(
             None, description="", alias="dbtMetrics"
         )  # relationship
         dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="dbtModels"
         )  # relationship
         view: Optional[View] = Field(None, description="", alias="view")  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         table_partition: Optional[TablePartition] = Field(
             None, description="", alias="tablePartition"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         data_quality_metric_dimensions: Optional[list[Metric]] = Field(
@@ -11744,14 +12878,17 @@
         if v != "Schema":
             raise ValueError("must be Schema")
         return v
 
     class Attributes(SQL.Attributes):
         table_count: Optional[int] = Field(None, description="", alias="tableCount")
         views_count: Optional[int] = Field(None, description="", alias="viewsCount")
+        snowflake_tags: Optional[list[SnowflakeTag]] = Field(
+            None, description="", alias="snowflakeTags"
+        )  # relationship
         materialised_views: Optional[list[MaterialisedView]] = Field(
             None, description="", alias="materialisedViews"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         dbt_sources: Optional[list[DbtSource]] = Field(
@@ -11774,23 +12911,29 @@
         )  # relationship
         tables: Optional[list[Table]] = Field(
             None, description="", alias="tables"
         )  # relationship
         database: Optional[Database] = Field(
             None, description="", alias="database"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         snowflake_pipes: Optional[list[SnowflakePipe]] = Field(
             None, description="", alias="snowflakePipes"
         )  # relationship
         snowflake_streams: Optional[list[SnowflakeStream]] = Field(
             None, description="", alias="snowflakeStreams"
         )  # relationship
         procedures: Optional[list[Procedure]] = Field(
             None, description="", alias="procedures"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         views: Optional[list[View]] = Field(
@@ -11949,44 +13092,50 @@
         )
         snowflake_stream_stale_after: Optional[datetime] = Field(
             None, description="", alias="snowflakeStreamStaleAfter"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        dbt_sources: Optional[list[DbtSource]] = Field(
+            None, description="", alias="dbtSources"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        sql_dbt_models: Optional[list[DbtModel]] = Field(
+            None, description="", alias="sqlDbtModels"
+        )  # relationship
+        sql_dbt_sources: Optional[list[DbtSource]] = Field(
+            None, description="", alias="sqlDBTSources"
+        )  # relationship
         dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="dbtModels"
         )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
         )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
 
     attributes: "SnowflakeStream.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
@@ -12071,44 +13220,50 @@
         )
         snowflake_pipe_notification_channel_name: Optional[str] = Field(
             None, description="", alias="snowflakePipeNotificationChannelName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        dbt_sources: Optional[list[DbtSource]] = Field(
+            None, description="", alias="dbtSources"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        sql_dbt_models: Optional[list[DbtModel]] = Field(
+            None, description="", alias="sqlDbtModels"
+        )  # relationship
+        sql_dbt_sources: Optional[list[DbtSource]] = Field(
+            None, description="", alias="sqlDBTSources"
+        )  # relationship
         dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="dbtModels"
         )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
         )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
 
     attributes: "SnowflakePipe.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
@@ -12157,44 +13312,50 @@
         return v
 
     class Attributes(SQL.Attributes):
         schema_count: Optional[int] = Field(None, description="", alias="schemaCount")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        dbt_sources: Optional[list[DbtSource]] = Field(
+            None, description="", alias="dbtSources"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        sql_dbt_models: Optional[list[DbtModel]] = Field(
+            None, description="", alias="sqlDbtModels"
+        )  # relationship
+        sql_dbt_sources: Optional[list[DbtSource]] = Field(
+            None, description="", alias="sqlDBTSources"
+        )  # relationship
         dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="dbtModels"
         )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
         )  # relationship
         schemas: Optional[list[Schema]] = Field(
             None, description="", alias="schemas"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls, name: str, connection_qualified_name: str
         ) -> Database.Attributes:
             if not name:
@@ -12290,44 +13451,50 @@
         return v
 
     class Attributes(SQL.Attributes):
         definition: str = Field(None, description="", alias="definition")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        dbt_sources: Optional[list[DbtSource]] = Field(
+            None, description="", alias="dbtSources"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        sql_dbt_models: Optional[list[DbtModel]] = Field(
+            None, description="", alias="sqlDbtModels"
+        )  # relationship
+        sql_dbt_sources: Optional[list[DbtSource]] = Field(
+            None, description="", alias="sqlDBTSources"
+        )  # relationship
         dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="dbtModels"
         )  # relationship
-        dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="dbtSources"
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
         )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
-        sql_dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="sqlDbtModels"
-        )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
-        sql_dbt_sources: Optional[list[DbtSource]] = Field(
-            None, description="", alias="sqlDBTSources"
-        )  # relationship
 
     attributes: "Procedure.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
@@ -12488,17 +13655,23 @@
         )  # relationship
         sql_dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="sqlDBTSources"
         )  # relationship
         dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="dbtModels"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         atlan_schema: Optional[Schema] = Field(
             None, description="", alias="atlanSchema"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
@@ -12732,47 +13905,53 @@
         )
         alias: Optional[str] = Field(None, description="", alias="alias")
         is_temporary: Optional[bool] = Field(None, description="", alias="isTemporary")
         definition: Optional[str] = Field(None, description="", alias="definition")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
-        dbt_models: Optional[list[DbtModel]] = Field(
-            None, description="", alias="dbtModels"
-        )  # relationship
         dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="dbtSources"
         )  # relationship
-        atlan_schema: Optional[Schema] = Field(
-            None, description="", alias="atlanSchema"
-        )  # relationship
         columns: Optional[list[Column]] = Field(
             None, description="", alias="columns"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
         readme: Optional[Readme] = Field(
             None, description="", alias="readme"
         )  # relationship
         meanings: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="meanings"
         )  # relationship
         sql_dbt_models: Optional[list[DbtModel]] = Field(
             None, description="", alias="sqlDbtModels"
         )  # relationship
-        output_from_processes: Optional[list[Process]] = Field(
-            None, description="", alias="outputFromProcesses"
-        )  # relationship
         sql_dbt_sources: Optional[list[DbtSource]] = Field(
             None, description="", alias="sqlDBTSources"
         )  # relationship
+        dbt_models: Optional[list[DbtModel]] = Field(
+            None, description="", alias="dbtModels"
+        )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        atlan_schema: Optional[Schema] = Field(
+            None, description="", alias="atlanSchema"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
 
     attributes: "MaterialisedView.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
@@ -13029,17 +14208,23 @@
         )
         gcs_object_retention_expiration_date: Optional[datetime] = Field(
             None, description="", alias="gcsObjectRetentionExpirationDate"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         gcs_bucket: Optional[GCSBucket] = Field(
             None, description="", alias="gcsBucket"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -13195,14 +14380,20 @@
         )
         gcs_bucket_retention_policy: Optional[str] = Field(
             None, description="", alias="gcsBucketRetentionPolicy"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         gcs_objects: Optional[list[GCSObject]] = Field(
             None, description="", alias="gcsObjects"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -13405,14 +14596,20 @@
         )
         adls_account_access_tier: Optional[ADLSAccessTier] = Field(
             None, description="", alias="adlsAccountAccessTier"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -13566,17 +14763,23 @@
         )
         adls_objects: Optional[list[ADLSObject]] = Field(
             None, description="", alias="adlsObjects"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         adls_account: Optional[ADLSAccount] = Field(
             None, description="", alias="adlsAccount"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -13891,14 +15094,20 @@
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         adls_container: Optional[ADLSContainer] = Field(
             None, description="", alias="adlsContainer"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -13980,17 +15189,23 @@
         )
         s3_bucket_versioning_enabled: Optional[bool] = Field(
             None, description="", alias="s3BucketVersioningEnabled"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         objects: Optional[list[S3Object]] = Field(
             None, description="", alias="objects"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -14217,14 +15432,20 @@
         )
         bucket: Optional[S3Bucket] = Field(
             None, description="", alias="bucket"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -14450,17 +15671,23 @@
         )
         kafka_topic_cleanup_policy: Optional[PowerbiEndorsement] = Field(
             None, description="", alias="kafkaTopicCleanupPolicy"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         kafka_consumer_groups: Optional[list[KafkaConsumerGroup]] = Field(
             None, description="", alias="kafkaConsumerGroups"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -14585,14 +15812,20 @@
         )
         kafka_topic_qualified_names: Optional[set[str]] = Field(
             None, description="", alias="kafkaTopicQualifiedNames"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         kafka_topics: Optional[list[KafkaTopic]] = Field(
             None, description="", alias="kafkaTopics"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -14611,14 +15844,491 @@
     attributes: "KafkaConsumerGroup.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
 
+class MCIncident(MonteCarlo):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MCIncident._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "mc_incident_id",
+        "mc_incident_type",
+        "mc_incident_sub_types",
+        "mc_incident_severity",
+        "mc_incident_state",
+        "mc_incident_warehouse",
+        "terms",
+    ]
+
+    @property
+    def mc_incident_id(self) -> Optional[str]:
+        return self.attributes.mc_incident_id
+
+    @mc_incident_id.setter
+    def mc_incident_id(self, mc_incident_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_incident_id = mc_incident_id
+
+    @property
+    def mc_incident_type(self) -> Optional[str]:
+        return self.attributes.mc_incident_type
+
+    @mc_incident_type.setter
+    def mc_incident_type(self, mc_incident_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_incident_type = mc_incident_type
+
+    @property
+    def mc_incident_sub_types(self) -> Optional[set[str]]:
+        return self.attributes.mc_incident_sub_types
+
+    @mc_incident_sub_types.setter
+    def mc_incident_sub_types(self, mc_incident_sub_types: Optional[set[str]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_incident_sub_types = mc_incident_sub_types
+
+    @property
+    def mc_incident_severity(self) -> Optional[str]:
+        return self.attributes.mc_incident_severity
+
+    @mc_incident_severity.setter
+    def mc_incident_severity(self, mc_incident_severity: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_incident_severity = mc_incident_severity
+
+    @property
+    def mc_incident_state(self) -> Optional[str]:
+        return self.attributes.mc_incident_state
+
+    @mc_incident_state.setter
+    def mc_incident_state(self, mc_incident_state: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_incident_state = mc_incident_state
+
+    @property
+    def mc_incident_warehouse(self) -> Optional[str]:
+        return self.attributes.mc_incident_warehouse
+
+    @mc_incident_warehouse.setter
+    def mc_incident_warehouse(self, mc_incident_warehouse: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_incident_warehouse = mc_incident_warehouse
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
+    type_name: str = Field("MCIncident", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MCIncident":
+            raise ValueError("must be MCIncident")
+        return v
+
+    class Attributes(MonteCarlo.Attributes):
+        mc_incident_id: Optional[str] = Field(
+            None, description="", alias="mcIncidentId"
+        )
+        mc_incident_type: Optional[str] = Field(
+            None, description="", alias="mcIncidentType"
+        )
+        mc_incident_sub_types: Optional[set[str]] = Field(
+            None, description="", alias="mcIncidentSubTypes"
+        )
+        mc_incident_severity: Optional[str] = Field(
+            None, description="", alias="mcIncidentSeverity"
+        )
+        mc_incident_state: Optional[str] = Field(
+            None, description="", alias="mcIncidentState"
+        )
+        mc_incident_warehouse: Optional[str] = Field(
+            None, description="", alias="mcIncidentWarehouse"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        mc_incident_assets: Optional[list[Asset]] = Field(
+            None, description="", alias="mcIncidentAssets"
+        )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_monitor: Optional[MCMonitor] = Field(
+            None, description="", alias="mcMonitor"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "MCIncident.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
+class MCMonitor(MonteCarlo):
+    """Description"""
+
+    def __setattr__(self, name, value):
+        if name in MCMonitor._convience_properties:
+            return object.__setattr__(self, name, value)
+        super().__setattr__(name, value)
+
+    _convience_properties: ClassVar[list[str]] = [
+        "mc_monitor_id",
+        "mc_monitor_status",
+        "mc_monitor_type",
+        "mc_monitor_warehouse",
+        "mc_monitor_schedule_type",
+        "mc_monitor_namespace",
+        "mc_monitor_rule_type",
+        "mc_monitor_rule_custom_sql",
+        "mc_monitor_rule_schedule_config",
+        "mc_monitor_rule_schedule_config_humanized",
+        "mc_monitor_alert_condition",
+        "mc_monitor_rule_next_execution_time",
+        "mc_monitor_rule_previous_execution_time",
+        "mc_monitor_rule_comparisons",
+        "mc_monitor_rule_is_snoozed",
+        "mc_monitor_breach_rate",
+        "mc_monitor_incident_count",
+        "terms",
+    ]
+
+    @property
+    def mc_monitor_id(self) -> Optional[str]:
+        return self.attributes.mc_monitor_id
+
+    @mc_monitor_id.setter
+    def mc_monitor_id(self, mc_monitor_id: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_id = mc_monitor_id
+
+    @property
+    def mc_monitor_status(self) -> Optional[str]:
+        return self.attributes.mc_monitor_status
+
+    @mc_monitor_status.setter
+    def mc_monitor_status(self, mc_monitor_status: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_status = mc_monitor_status
+
+    @property
+    def mc_monitor_type(self) -> Optional[str]:
+        return self.attributes.mc_monitor_type
+
+    @mc_monitor_type.setter
+    def mc_monitor_type(self, mc_monitor_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_type = mc_monitor_type
+
+    @property
+    def mc_monitor_warehouse(self) -> Optional[str]:
+        return self.attributes.mc_monitor_warehouse
+
+    @mc_monitor_warehouse.setter
+    def mc_monitor_warehouse(self, mc_monitor_warehouse: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_warehouse = mc_monitor_warehouse
+
+    @property
+    def mc_monitor_schedule_type(self) -> Optional[str]:
+        return self.attributes.mc_monitor_schedule_type
+
+    @mc_monitor_schedule_type.setter
+    def mc_monitor_schedule_type(self, mc_monitor_schedule_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_schedule_type = mc_monitor_schedule_type
+
+    @property
+    def mc_monitor_namespace(self) -> Optional[str]:
+        return self.attributes.mc_monitor_namespace
+
+    @mc_monitor_namespace.setter
+    def mc_monitor_namespace(self, mc_monitor_namespace: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_namespace = mc_monitor_namespace
+
+    @property
+    def mc_monitor_rule_type(self) -> Optional[str]:
+        return self.attributes.mc_monitor_rule_type
+
+    @mc_monitor_rule_type.setter
+    def mc_monitor_rule_type(self, mc_monitor_rule_type: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_rule_type = mc_monitor_rule_type
+
+    @property
+    def mc_monitor_rule_custom_sql(self) -> Optional[str]:
+        return self.attributes.mc_monitor_rule_custom_sql
+
+    @mc_monitor_rule_custom_sql.setter
+    def mc_monitor_rule_custom_sql(self, mc_monitor_rule_custom_sql: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_rule_custom_sql = mc_monitor_rule_custom_sql
+
+    @property
+    def mc_monitor_rule_schedule_config(self) -> Optional[MCRuleSchedule]:
+        return self.attributes.mc_monitor_rule_schedule_config
+
+    @mc_monitor_rule_schedule_config.setter
+    def mc_monitor_rule_schedule_config(
+        self, mc_monitor_rule_schedule_config: Optional[MCRuleSchedule]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_rule_schedule_config = (
+            mc_monitor_rule_schedule_config
+        )
+
+    @property
+    def mc_monitor_rule_schedule_config_humanized(self) -> Optional[str]:
+        return self.attributes.mc_monitor_rule_schedule_config_humanized
+
+    @mc_monitor_rule_schedule_config_humanized.setter
+    def mc_monitor_rule_schedule_config_humanized(
+        self, mc_monitor_rule_schedule_config_humanized: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_rule_schedule_config_humanized = (
+            mc_monitor_rule_schedule_config_humanized
+        )
+
+    @property
+    def mc_monitor_alert_condition(self) -> Optional[str]:
+        return self.attributes.mc_monitor_alert_condition
+
+    @mc_monitor_alert_condition.setter
+    def mc_monitor_alert_condition(self, mc_monitor_alert_condition: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_alert_condition = mc_monitor_alert_condition
+
+    @property
+    def mc_monitor_rule_next_execution_time(self) -> Optional[datetime]:
+        return self.attributes.mc_monitor_rule_next_execution_time
+
+    @mc_monitor_rule_next_execution_time.setter
+    def mc_monitor_rule_next_execution_time(
+        self, mc_monitor_rule_next_execution_time: Optional[datetime]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_rule_next_execution_time = (
+            mc_monitor_rule_next_execution_time
+        )
+
+    @property
+    def mc_monitor_rule_previous_execution_time(self) -> Optional[datetime]:
+        return self.attributes.mc_monitor_rule_previous_execution_time
+
+    @mc_monitor_rule_previous_execution_time.setter
+    def mc_monitor_rule_previous_execution_time(
+        self, mc_monitor_rule_previous_execution_time: Optional[datetime]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_rule_previous_execution_time = (
+            mc_monitor_rule_previous_execution_time
+        )
+
+    @property
+    def mc_monitor_rule_comparisons(self) -> Optional[list[MCRuleComparison]]:
+        return self.attributes.mc_monitor_rule_comparisons
+
+    @mc_monitor_rule_comparisons.setter
+    def mc_monitor_rule_comparisons(
+        self, mc_monitor_rule_comparisons: Optional[list[MCRuleComparison]]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_rule_comparisons = mc_monitor_rule_comparisons
+
+    @property
+    def mc_monitor_rule_is_snoozed(self) -> Optional[bool]:
+        return self.attributes.mc_monitor_rule_is_snoozed
+
+    @mc_monitor_rule_is_snoozed.setter
+    def mc_monitor_rule_is_snoozed(self, mc_monitor_rule_is_snoozed: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_rule_is_snoozed = mc_monitor_rule_is_snoozed
+
+    @property
+    def mc_monitor_breach_rate(self) -> Optional[float]:
+        return self.attributes.mc_monitor_breach_rate
+
+    @mc_monitor_breach_rate.setter
+    def mc_monitor_breach_rate(self, mc_monitor_breach_rate: Optional[float]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_breach_rate = mc_monitor_breach_rate
+
+    @property
+    def mc_monitor_incident_count(self) -> Optional[int]:
+        return self.attributes.mc_monitor_incident_count
+
+    @mc_monitor_incident_count.setter
+    def mc_monitor_incident_count(self, mc_monitor_incident_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.mc_monitor_incident_count = mc_monitor_incident_count
+
+    @property
+    def terms(self) -> list[AtlasGlossaryTerm]:
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        return [] if self.attributes.meanings is None else self.attributes.meanings
+
+    @terms.setter
+    def terms(self, terms: list[AtlasGlossaryTerm]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.meanings = terms
+
+    type_name: str = Field("MCMonitor", allow_mutation=False)
+
+    @validator("type_name")
+    def validate_type_name(cls, v):
+        if v != "MCMonitor":
+            raise ValueError("must be MCMonitor")
+        return v
+
+    class Attributes(MonteCarlo.Attributes):
+        mc_monitor_id: Optional[str] = Field(None, description="", alias="mcMonitorId")
+        mc_monitor_status: Optional[str] = Field(
+            None, description="", alias="mcMonitorStatus"
+        )
+        mc_monitor_type: Optional[str] = Field(
+            None, description="", alias="mcMonitorType"
+        )
+        mc_monitor_warehouse: Optional[str] = Field(
+            None, description="", alias="mcMonitorWarehouse"
+        )
+        mc_monitor_schedule_type: Optional[str] = Field(
+            None, description="", alias="mcMonitorScheduleType"
+        )
+        mc_monitor_namespace: Optional[str] = Field(
+            None, description="", alias="mcMonitorNamespace"
+        )
+        mc_monitor_rule_type: Optional[str] = Field(
+            None, description="", alias="mcMonitorRuleType"
+        )
+        mc_monitor_rule_custom_sql: Optional[str] = Field(
+            None, description="", alias="mcMonitorRuleCustomSql"
+        )
+        mc_monitor_rule_schedule_config: Optional[MCRuleSchedule] = Field(
+            None, description="", alias="mcMonitorRuleScheduleConfig"
+        )
+        mc_monitor_rule_schedule_config_humanized: Optional[str] = Field(
+            None, description="", alias="mcMonitorRuleScheduleConfigHumanized"
+        )
+        mc_monitor_alert_condition: Optional[str] = Field(
+            None, description="", alias="mcMonitorAlertCondition"
+        )
+        mc_monitor_rule_next_execution_time: Optional[datetime] = Field(
+            None, description="", alias="mcMonitorRuleNextExecutionTime"
+        )
+        mc_monitor_rule_previous_execution_time: Optional[datetime] = Field(
+            None, description="", alias="mcMonitorRulePreviousExecutionTime"
+        )
+        mc_monitor_rule_comparisons: Optional[list[MCRuleComparison]] = Field(
+            None, description="", alias="mcMonitorRuleComparisons"
+        )
+        mc_monitor_rule_is_snoozed: Optional[bool] = Field(
+            None, description="", alias="mcMonitorRuleIsSnoozed"
+        )
+        mc_monitor_breach_rate: Optional[float] = Field(
+            None, description="", alias="mcMonitorBreachRate"
+        )
+        mc_monitor_incident_count: Optional[int] = Field(
+            None, description="", alias="mcMonitorIncidentCount"
+        )
+        input_to_processes: Optional[list[Process]] = Field(
+            None, description="", alias="inputToProcesses"
+        )  # relationship
+        mc_monitor_assets: Optional[list[Asset]] = Field(
+            None, description="", alias="mcMonitorAssets"
+        )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        output_from_processes: Optional[list[Process]] = Field(
+            None, description="", alias="outputFromProcesses"
+        )  # relationship
+
+    attributes: "MCMonitor.Attributes" = Field(
+        None,
+        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
+        "type, so are described in the sub-types of this schema.\n",
+    )
+
+
 class MetabaseQuestion(Metabase):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in MetabaseQuestion._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
@@ -14689,17 +16399,23 @@
         )
         metabase_query: Optional[str] = Field(
             None, description="", alias="metabaseQuery"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         metabase_dashboards: Optional[list[MetabaseDashboard]] = Field(
             None, description="", alias="metabaseDashboards"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -14812,17 +16528,23 @@
         )
         metabase_is_personal_collection: Optional[bool] = Field(
             None, description="", alias="metabaseIsPersonalCollection"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         metabase_dashboards: Optional[list[MetabaseDashboard]] = Field(
             None, description="", alias="metabaseDashboards"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -14891,14 +16613,20 @@
     class Attributes(Metabase.Attributes):
         metabase_question_count: Optional[int] = Field(
             None, description="", alias="metabaseQuestionCount"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -14991,17 +16719,23 @@
         )
         quick_sight_dashboards: Optional[list[QuickSightDashboard]] = Field(
             None, description="", alias="quickSightDashboards"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         quick_sight_analyses: Optional[list[QuickSightAnalysis]] = Field(
             None, description="", alias="quickSightAnalyses"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -15074,14 +16808,20 @@
     class Attributes(QuickSight.Attributes):
         quick_sight_dashboard_qualified_name: Optional[str] = Field(
             None, description="", alias="quickSightDashboardQualifiedName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -15154,14 +16894,20 @@
     class Attributes(QuickSight.Attributes):
         quick_sight_analysis_qualified_name: Optional[str] = Field(
             None, description="", alias="quickSightAnalysisQualifiedName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         quick_sight_analysis: Optional[QuickSightAnalysis] = Field(
             None, description="", alias="quickSightAnalysis"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -15250,14 +16996,20 @@
         )
         quick_sight_dataset_qualified_name: Optional[str] = Field(
             None, description="", alias="quickSightDatasetQualifiedName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         quick_sight_dataset: Optional[QuickSightDataset] = Field(
             None, description="", alias="quickSightDataset"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -15385,14 +17137,20 @@
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]] = Field(
             None, description="", alias="quickSightAnalysisVisuals"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -15483,22 +17241,28 @@
         )
         quick_sight_dashboard_last_published_time: Optional[datetime] = Field(
             None, description="", alias="quickSightDashboardLastPublishedTime"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         quick_sight_dashboard_folders: Optional[list[QuickSightFolder]] = Field(
             None, description="", alias="quickSightDashboardFolders"
         )  # relationship
         quick_sight_dashboard_visuals: Optional[
             list[QuickSightDashboardVisual]
         ] = Field(
             None, description="", alias="quickSightDashboardVisuals"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -15586,17 +17350,23 @@
         )
         quick_sight_dataset_column_count: Optional[int] = Field(
             None, description="", alias="quickSightDatasetColumnCount"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         quick_sight_dataset_folders: Optional[list[QuickSightFolder]] = Field(
             None, description="", alias="quickSightDatasetFolders"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         quick_sight_dataset_fields: Optional[list[QuickSightDatasetField]] = Field(
             None, description="", alias="quickSightDatasetFields"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -15651,17 +17421,23 @@
             raise ValueError("must be ThoughtspotLiveboard")
         return v
 
     class Attributes(Thoughtspot.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         thoughtspot_dashlets: Optional[list[ThoughtspotDashlet]] = Field(
             None, description="", alias="thoughtspotDashlets"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -15745,17 +17521,23 @@
         )
         thoughtspot_liveboard_qualified_name: Optional[str] = Field(
             None, description="", alias="thoughtspotLiveboardQualifiedName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         thoughtspot_liveboard: Optional[ThoughtspotLiveboard] = Field(
             None, description="", alias="thoughtspotLiveboard"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -15807,14 +17589,20 @@
             raise ValueError("must be ThoughtspotAnswer")
         return v
 
     class Attributes(Thoughtspot.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -15924,17 +17712,23 @@
         )  # relationship
         tiles: Optional[list[PowerBITile]] = Field(
             None, description="", alias="tiles"
         )  # relationship
         workspace: Optional[PowerBIWorkspace] = Field(
             None, description="", alias="workspace"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         pages: Optional[list[PowerBIPage]] = Field(
             None, description="", alias="pages"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -16047,14 +17841,20 @@
         )
         power_b_i_is_external_measure: Optional[bool] = Field(
             None, description="", alias="powerBIIsExternalMeasure"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -16197,14 +17997,20 @@
         )
         power_b_i_column_summarize_by: Optional[str] = Field(
             None, description="", alias="powerBIColumnSummarizeBy"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -16338,17 +18144,23 @@
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         measures: Optional[list[PowerBIMeasure]] = Field(
             None, description="", alias="measures"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         columns: Optional[list[PowerBIColumn]] = Field(
             None, description="", alias="columns"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -16431,17 +18243,23 @@
         )
         dashboard_qualified_name: Optional[str] = Field(
             None, description="", alias="dashboardQualifiedName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         report: Optional[PowerBIReport] = Field(
             None, description="", alias="report"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -16513,14 +18331,20 @@
     class Attributes(PowerBI.Attributes):
         connection_details: Optional[dict[str, str]] = Field(
             None, description="", alias="connectionDetails"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         datasets: Optional[list[PowerBIDataset]] = Field(
             None, description="", alias="datasets"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -16642,14 +18466,20 @@
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         reports: Optional[list[PowerBIReport]] = Field(
             None, description="", alias="reports"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         datasets: Optional[list[PowerBIDataset]] = Field(
             None, description="", alias="datasets"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -16736,44 +18566,50 @@
         workspace_qualified_name: Optional[str] = Field(
             None, description="", alias="workspaceQualifiedName"
         )
         web_url: Optional[str] = Field(None, description="", alias="webUrl")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
-        tiles: Optional[list[PowerBITile]] = Field(
-            None, description="", alias="tiles"
-        )  # relationship
         reports: Optional[list[PowerBIReport]] = Field(
             None, description="", alias="reports"
         )  # relationship
         workspace: Optional[PowerBIWorkspace] = Field(
             None, description="", alias="workspace"
         )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        dataflows: Optional[list[PowerBIDataflow]] = Field(
+            None, description="", alias="dataflows"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        tiles: Optional[list[PowerBITile]] = Field(
+            None, description="", alias="tiles"
+        )  # relationship
         tables: Optional[list[PowerBITable]] = Field(
             None, description="", alias="tables"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         datasources: Optional[list[PowerBIDatasource]] = Field(
             None, description="", alias="datasources"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        dataflows: Optional[list[PowerBIDataflow]] = Field(
-            None, description="", alias="dataflows"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
     attributes: "PowerBIDataset.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
@@ -16857,14 +18693,20 @@
         )  # relationship
         tiles: Optional[list[PowerBITile]] = Field(
             None, description="", alias="tiles"
         )  # relationship
         workspace: Optional[PowerBIWorkspace] = Field(
             None, description="", alias="workspace"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -16945,14 +18787,20 @@
         web_url: Optional[str] = Field(None, description="", alias="webUrl")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         workspace: Optional[PowerBIWorkspace] = Field(
             None, description="", alias="workspace"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         datasets: Optional[list[PowerBIDataset]] = Field(
             None, description="", alias="datasets"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -17035,17 +18883,23 @@
         )
         report_qualified_name: Optional[str] = Field(
             None, description="", alias="reportQualifiedName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         report: Optional[PowerBIReport] = Field(
             None, description="", alias="report"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -17129,14 +18983,20 @@
         )
         preset_chart_form_data: Optional[dict[str, str]] = Field(
             None, description="", alias="presetChartFormData"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         preset_dashboard: Optional[PresetDashboard] = Field(
             None, description="", alias="presetDashboard"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -17235,14 +19095,20 @@
         )
         preset_dataset_type: Optional[str] = Field(
             None, description="", alias="presetDatasetType"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         preset_dashboard: Optional[PresetDashboard] = Field(
             None, description="", alias="presetDashboard"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -17400,17 +19266,23 @@
         )
         preset_datasets: Optional[list[PresetDataset]] = Field(
             None, description="", alias="presetDatasets"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         preset_charts: Optional[list[PresetChart]] = Field(
             None, description="", alias="presetCharts"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         preset_workspace: Optional[PresetWorkspace] = Field(
             None, description="", alias="presetWorkspace"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -17610,14 +19482,20 @@
         )
         preset_dashboards: Optional[list[PresetDashboard]] = Field(
             None, description="", alias="presetDashboards"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -17767,17 +19645,23 @@
         )
         mode_is_shared: Optional[bool] = Field(
             None, description="", alias="modeIsShared"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         mode_collections: Optional[list[ModeCollection]] = Field(
             None, description="", alias="modeCollections"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -17863,14 +19747,20 @@
         )
         mode_charts: Optional[list[ModeChart]] = Field(
             None, description="", alias="modeCharts"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         mode_report: Optional[ModeReport] = Field(
             None, description="", alias="modeReport"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -17939,14 +19829,20 @@
     class Attributes(Mode.Attributes):
         mode_chart_type: Optional[str] = Field(
             None, description="", alias="modeChartType"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -18015,17 +19911,23 @@
     class Attributes(Mode.Attributes):
         mode_collection_count: Optional[int] = Field(
             None, description="", alias="modeCollectionCount"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         mode_collections: Optional[list[ModeCollection]] = Field(
             None, description="", alias="modeCollections"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -18105,14 +20007,20 @@
         )
         mode_collection_state: Optional[str] = Field(
             None, description="", alias="modeCollectionState"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         mode_workspace: Optional[ModeWorkspace] = Field(
             None, description="", alias="modeWorkspace"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -18198,17 +20106,23 @@
         )
         sigma_dataset_name: Optional[str] = Field(
             None, description="", alias="sigmaDatasetName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         sigma_dataset: Optional[SigmaDataset] = Field(
             None, description="", alias="sigmaDataset"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -18274,14 +20188,20 @@
     class Attributes(Sigma.Attributes):
         sigma_dataset_column_count: Optional[int] = Field(
             None, description="", alias="sigmaDatasetColumnCount"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -18350,17 +20270,23 @@
     class Attributes(Sigma.Attributes):
         sigma_page_count: Optional[int] = Field(
             None, description="", alias="sigmaPageCount"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         sigma_pages: Optional[list[SigmaPage]] = Field(
             None, description="", alias="sigmaPages"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -18448,17 +20374,23 @@
         )
         sigma_data_element_field_formula: Optional[str] = Field(
             None, description="", alias="sigmaDataElementFieldFormula"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         sigma_data_element: Optional[SigmaDataElement] = Field(
             None, description="", alias="sigmaDataElement"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -18527,14 +20459,20 @@
         )
         sigma_data_elements: Optional[list[SigmaDataElement]] = Field(
             None, description="", alias="sigmaDataElements"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         sigma_workbook: Optional[SigmaWorkbook] = Field(
             None, description="", alias="sigmaWorkbook"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -18633,14 +20571,20 @@
         )
         sigma_data_element_field_count: Optional[int] = Field(
             None, description="", alias="sigmaDataElementFieldCount"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -18715,14 +20659,20 @@
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         qlik_datasets: Optional[list[QlikDataset]] = Field(
             None, description="", alias="qlikDatasets"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         qlik_apps: Optional[list[QlikApp]] = Field(
             None, description="", alias="qlikApps"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -18847,17 +20797,23 @@
         )
         qlik_app_static_byte_size: Optional[int] = Field(
             None, description="", alias="qlikAppStaticByteSize"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         qlik_space: Optional[QlikSpace] = Field(
             None, description="", alias="qlikSpace"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         qlik_sheets: Optional[list[QlikSheet]] = Field(
             None, description="", alias="qlikSheets"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -18968,17 +20924,23 @@
         )
         qlik_chart_type: Optional[str] = Field(
             None, description="", alias="qlikChartType"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         qlik_sheet: Optional[QlikSheet] = Field(
             None, description="", alias="qlikSheet"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -19086,17 +21048,23 @@
         )
         qlik_dataset_subtype: Optional[str] = Field(
             None, description="", alias="qlikDatasetSubtype"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         qlik_space: Optional[QlikSpace] = Field(
             None, description="", alias="qlikSpace"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -19165,17 +21133,23 @@
         )
         qlik_app: Optional[QlikApp] = Field(
             None, description="", alias="qlikApp"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         qlik_charts: Optional[list[QlikChart]] = Field(
             None, description="", alias="qlikCharts"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -19301,23 +21275,29 @@
         )
         project_hierarchy: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="projectHierarchy"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         worksheets: Optional[list[TableauWorksheet]] = Field(
             None, description="", alias="worksheets"
         )  # relationship
         datasources: Optional[list[TableauDatasource]] = Field(
             None, description="", alias="datasources"
         )  # relationship
         project: Optional[TableauProject] = Field(
             None, description="", alias="project"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -19618,20 +21598,26 @@
         )
         datasource_field_type: Optional[str] = Field(
             None, description="", alias="datasourceFieldType"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         worksheets: Optional[list[TableauWorksheet]] = Field(
             None, description="", alias="worksheets"
         )  # relationship
         datasource: Optional[TableauDatasource] = Field(
             None, description="", alias="datasource"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -19835,20 +21821,26 @@
         formula: Optional[str] = Field(None, description="", alias="formula")
         upstream_fields: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="upstreamFields"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         worksheets: Optional[list[TableauWorksheet]] = Field(
             None, description="", alias="worksheets"
         )  # relationship
         datasource: Optional[TableauDatasource] = Field(
             None, description="", alias="datasource"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -19960,44 +21952,50 @@
         )
         project_hierarchy: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="projectHierarchy"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        parent_project: Optional[TableauProject] = Field(
+            None, description="", alias="parentProject"
+        )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
         workbooks: Optional[list[TableauWorkbook]] = Field(
             None, description="", alias="workbooks"
         )  # relationship
         site: Optional[TableauSite] = Field(
             None, description="", alias="site"
         )  # relationship
-        parent_project: Optional[TableauProject] = Field(
-            None, description="", alias="parentProject"
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
         )  # relationship
         datasources: Optional[list[TableauDatasource]] = Field(
             None, description="", alias="datasources"
         )  # relationship
         flows: Optional[list[TableauFlow]] = Field(
             None, description="", alias="flows"
         )  # relationship
         child_projects: Optional[list[TableauProject]] = Field(
             None, description="", alias="childProjects"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
     attributes: "TableauProject.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
@@ -20097,17 +22095,23 @@
         )
         project_hierarchy: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="projectHierarchy"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         project: Optional[TableauProject] = Field(
             None, description="", alias="project"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -20159,17 +22163,23 @@
             raise ValueError("must be TableauSite")
         return v
 
     class Attributes(Tableau.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         projects: Optional[list[TableauProject]] = Field(
             None, description="", alias="projects"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -20406,17 +22416,23 @@
         )
         workbook: Optional[TableauWorkbook] = Field(
             None, description="", alias="workbook"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         project: Optional[TableauProject] = Field(
             None, description="", alias="project"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -20548,17 +22564,23 @@
         )
         workbook: Optional[TableauWorkbook] = Field(
             None, description="", alias="workbook"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         worksheets: Optional[list[TableauWorksheet]] = Field(
             None, description="", alias="worksheets"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -20712,17 +22734,23 @@
         )
         output_steps: Optional[list[dict[str, str]]] = Field(
             None, description="", alias="outputSteps"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         project: Optional[TableauProject] = Field(
             None, description="", alias="project"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -20851,17 +22879,23 @@
         )
         workbook: Optional[TableauWorkbook] = Field(
             None, description="", alias="workbook"
         )  # relationship
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         datasource_fields: Optional[list[TableauDatasourceField]] = Field(
             None, description="", alias="datasourceFields"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -21041,38 +23075,44 @@
         source_query_id: Optional[int] = Field(
             None, description="", alias="sourceQueryId"
         )
         model_name: Optional[str] = Field(None, description="", alias="modelName")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
-        folder: Optional[LookerFolder] = Field(
-            None, description="", alias="folder"
-        )  # relationship
         query: Optional[LookerQuery] = Field(
             None, description="", alias="query"
         )  # relationship
+        readme: Optional[Readme] = Field(
+            None, description="", alias="readme"
+        )  # relationship
+        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
+            None, description="", alias="meanings"
+        )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        folder: Optional[LookerFolder] = Field(
+            None, description="", alias="folder"
+        )  # relationship
         tile: Optional[LookerTile] = Field(
             None, description="", alias="tile"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         model: Optional[LookerModel] = Field(
             None, description="", alias="model"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
-        readme: Optional[Readme] = Field(
-            None, description="", alias="readme"
-        )  # relationship
-        meanings: Optional[list[AtlasGlossaryTerm]] = Field(
-            None, description="", alias="meanings"
-        )  # relationship
         dashboard: Optional[LookerDashboard] = Field(
             None, description="", alias="dashboard"
         )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
@@ -21217,17 +23257,23 @@
         )  # relationship
         tiles: Optional[list[LookerTile]] = Field(
             None, description="", alias="tiles"
         )  # relationship
         looks: Optional[list[LookerLook]] = Field(
             None, description="", alias="looks"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         folder: Optional[LookerFolder] = Field(
             None, description="", alias="folder"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -21338,14 +23384,20 @@
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         looks: Optional[list[LookerLook]] = Field(
             None, description="", alias="looks"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -21490,17 +23542,23 @@
             None, description="", alias="resultMakerID"
         )
         subtitle_text: Optional[str] = Field(None, description="", alias="subtitleText")
         look_id: Optional[int] = Field(None, description="", alias="lookId")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         query: Optional[LookerQuery] = Field(
             None, description="", alias="query"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -21576,35 +23634,41 @@
         )  # relationship
         explores: Optional[list[LookerExplore]] = Field(
             None, description="", alias="explores"
         )  # relationship
         project: Optional[LookerProject] = Field(
             None, description="", alias="project"
         )  # relationship
-        links: Optional[list[Link]] = Field(
-            None, description="", alias="links"
-        )  # relationship
-        metrics: Optional[list[Metric]] = Field(
-            None, description="", alias="metrics"
-        )  # relationship
         readme: Optional[Readme] = Field(
             None, description="", alias="readme"
         )  # relationship
-        fields: Optional[list[LookerField]] = Field(
-            None, description="", alias="fields"
-        )  # relationship
         look: Optional[LookerLook] = Field(
             None, description="", alias="look"
         )  # relationship
         queries: Optional[list[LookerQuery]] = Field(
             None, description="", alias="queries"
         )  # relationship
         meanings: Optional[list[AtlasGlossaryTerm]] = Field(
             None, description="", alias="meanings"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
+        links: Optional[list[Link]] = Field(
+            None, description="", alias="links"
+        )  # relationship
+        metrics: Optional[list[Metric]] = Field(
+            None, description="", alias="metrics"
+        )  # relationship
+        fields: Optional[list[LookerField]] = Field(
+            None, description="", alias="fields"
+        )  # relationship
         output_from_processes: Optional[list[Process]] = Field(
             None, description="", alias="outputFromProcesses"
         )  # relationship
 
     attributes: "LookerModel.Attributes" = Field(
         None,
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
@@ -21708,17 +23772,23 @@
         view_name: Optional[str] = Field(None, description="", alias="viewName")
         sql_table_name: Optional[str] = Field(
             None, description="", alias="sqlTableName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         project: Optional[LookerProject] = Field(
             None, description="", alias="project"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         model: Optional[LookerModel] = Field(
             None, description="", alias="model"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -21779,17 +23849,23 @@
     class Attributes(Looker.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         models: Optional[list[LookerModel]] = Field(
             None, description="", alias="models"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         explores: Optional[list[LookerExplore]] = Field(
             None, description="", alias="explores"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -21907,14 +23983,20 @@
         )  # relationship
         tiles: Optional[list[LookerTile]] = Field(
             None, description="", alias="tiles"
         )  # relationship
         looks: Optional[list[LookerLook]] = Field(
             None, description="", alias="looks"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         model: Optional[LookerModel] = Field(
             None, description="", alias="model"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -22068,20 +24150,26 @@
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         view: Optional[LookerView] = Field(
             None, description="", alias="view"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         explore: Optional[LookerExplore] = Field(
             None, description="", alias="explore"
         )  # relationship
         project: Optional[LookerProject] = Field(
             None, description="", alias="project"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         model: Optional[LookerModel] = Field(
             None, description="", alias="model"
         )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -22148,17 +24236,23 @@
         return v
 
     class Attributes(Looker.Attributes):
         project_name: Optional[str] = Field(None, description="", alias="projectName")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         project: Optional[LookerProject] = Field(
             None, description="", alias="project"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -22229,14 +24323,20 @@
     class Attributes(Redash.Attributes):
         redash_dashboard_widget_count: Optional[int] = Field(
             None, description="", alias="redashDashboardWidgetCount"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -22382,17 +24482,23 @@
         )
         redash_query_schedule_humanized: Optional[str] = Field(
             None, description="", alias="redashQueryScheduleHumanized"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         redash_visualizations: Optional[list[RedashVisualization]] = Field(
             None, description="", alias="redashVisualizations"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -22486,14 +24592,20 @@
         )
         redash_query_qualified_name: Optional[str] = Field(
             None, description="", alias="redashQueryQualifiedName"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -22596,20 +24708,26 @@
         is_custom: Optional[bool] = Field(None, description="", alias="isCustom")
         is_mergable: Optional[bool] = Field(None, description="", alias="isMergable")
         is_queryable: Optional[bool] = Field(None, description="", alias="isQueryable")
         field_count: Optional[int] = Field(None, description="", alias="fieldCount")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         organization: Optional[SalesforceOrganization] = Field(
             None, description="", alias="organization"
         )  # relationship
         lookup_fields: Optional[list[SalesforceField]] = Field(
             None, description="", alias="lookupFields"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -22872,17 +24990,23 @@
         )
         default_value_formula: Optional[str] = Field(
             None, description="", alias="defaultValueFormula"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         lookup_objects: Optional[list[SalesforceObject]] = Field(
             None, description="", alias="lookupObjects"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -22952,17 +25076,23 @@
         source_id: Optional[str] = Field(None, description="", alias="sourceId")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         reports: Optional[list[SalesforceReport]] = Field(
             None, description="", alias="reports"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         objects: Optional[list[SalesforceObject]] = Field(
             None, description="", alias="objects"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -23058,17 +25188,23 @@
         report_count: Optional[int] = Field(None, description="", alias="reportCount")
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
         reports: Optional[list[SalesforceReport]] = Field(
             None, description="", alias="reports"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         organization: Optional[SalesforceOrganization] = Field(
             None, description="", alias="organization"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -23160,17 +25296,23 @@
         )
         detail_columns: Optional[set[str]] = Field(
             None, description="", alias="detailColumns"
         )
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         organization: Optional[SalesforceOrganization] = Field(
             None, description="", alias="organization"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
             None, description="", alias="metrics"
         )  # relationship
         readme: Optional[Readme] = Field(
@@ -23225,17 +25367,23 @@
             raise ValueError("must be QlikStream")
         return v
 
     class Attributes(QlikSpace.Attributes):
         input_to_processes: Optional[list[Process]] = Field(
             None, description="", alias="inputToProcesses"
         )  # relationship
+        mc_monitors: Optional[list[MCMonitor]] = Field(
+            None, description="", alias="mcMonitors"
+        )  # relationship
         qlik_datasets: Optional[list[QlikDataset]] = Field(
             None, description="", alias="qlikDatasets"
         )  # relationship
+        mc_incidents: Optional[list[MCIncident]] = Field(
+            None, description="", alias="mcIncidents"
+        )  # relationship
         links: Optional[list[Link]] = Field(
             None, description="", alias="links"
         )  # relationship
         qlik_apps: Optional[list[QlikApp]] = Field(
             None, description="", alias="qlikApps"
         )  # relationship
         metrics: Optional[list[Metric]] = Field(
@@ -23317,14 +25465,16 @@
 
 Resource.Attributes.update_forward_refs()
 
 Insight.Attributes.update_forward_refs()
 
 API.Attributes.update_forward_refs()
 
+Tag.Attributes.update_forward_refs()
+
 SQL.Attributes.update_forward_refs()
 
 DataStudio.Attributes.update_forward_refs()
 
 GCS.Attributes.update_forward_refs()
 
 DataStudioAsset.Attributes.update_forward_refs()
@@ -23333,14 +25483,16 @@
 
 S3.Attributes.update_forward_refs()
 
 DbtColumnProcess.Attributes.update_forward_refs()
 
 Kafka.Attributes.update_forward_refs()
 
+MonteCarlo.Attributes.update_forward_refs()
+
 Metric.Attributes.update_forward_refs()
 
 Metabase.Attributes.update_forward_refs()
 
 QuickSight.Attributes.update_forward_refs()
 
 Thoughtspot.Attributes.update_forward_refs()
@@ -23379,14 +25531,16 @@
 
 Link.Attributes.update_forward_refs()
 
 APISpec.Attributes.update_forward_refs()
 
 APIPath.Attributes.update_forward_refs()
 
+SnowflakeTag.Attributes.update_forward_refs()
+
 TablePartition.Attributes.update_forward_refs()
 
 Table.Attributes.update_forward_refs()
 
 Query.Attributes.update_forward_refs()
 
 Column.Attributes.update_forward_refs()
@@ -23419,14 +25573,18 @@
 
 S3Object.Attributes.update_forward_refs()
 
 KafkaTopic.Attributes.update_forward_refs()
 
 KafkaConsumerGroup.Attributes.update_forward_refs()
 
+MCIncident.Attributes.update_forward_refs()
+
+MCMonitor.Attributes.update_forward_refs()
+
 MetabaseQuestion.Attributes.update_forward_refs()
 
 MetabaseCollection.Attributes.update_forward_refs()
 
 MetabaseDashboard.Attributes.update_forward_refs()
 
 QuickSightFolder.Attributes.update_forward_refs()
```

### Comparing `pyatlan-0.0.31/pyatlan/model/core.py` & `pyatlan-0.0.32/pyatlan/model/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         value.replace("URL", "Url").replace("DBT", "Dbt").replace("GDPR", "Gdpr")[1:]
     ):
         if c in "ABCDEFGHIJKLMNOPQRSTUVWXYZ":
             res.append("_")
             res.append(c.lower())
         else:
             res.append(c)
-    return "".join(res)
+    return "".join(res).replace(" _", "_").replace(" ", "_")
 
 
 class ClassificationName:
     def __init__(self, display_text: str):
         from pyatlan.cache.classification_cache import ClassificationCache
 
         if not ClassificationCache.get_id_for_name(display_text):
```

### Comparing `pyatlan-0.0.31/pyatlan/model/lineage.py` & `pyatlan-0.0.32/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.31/pyatlan/model/response.py` & `pyatlan-0.0.32/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.31/pyatlan/model/role.py` & `pyatlan-0.0.32/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.31/pyatlan/model/search.py` & `pyatlan-0.0.32/pyatlan/model/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         obj = str.__new__(cls, value)
         obj._value_ = value
         obj.attribute_type = attribute_type
         return obj
 
 
 class TermAttributes(Attributes):
-
     CONNECTOR_NAME = ("connectorName", AtlanConnectorType)
     CATEGORIES = ("__categories", StrictStr)
     CREATE_TIME_AS_TIMESTAMP = ("__timestamp", datetime)
     CREATED_BY = ("__createdBy", StrictStr)
     GLOSSARY = ("__glossary", StrictStr)
     GUID = ("__guid", StrictStr)
     HAS_LINEAGE = ("__hasLineage", StrictBool)
@@ -173,14 +172,28 @@
 @dataclass(config=ConfigDict(smart_union=True, extra="forbid"))  # type: ignore
 class Exists(Query):
     field: str
     type_name: Literal["exists"] = "exists"
 
     @classmethod
     @validate_arguments()
+    def with_custom_metadata(cls, set_name: StrictStr, attr_name: StrictStr):
+        from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+
+        if attr_id := CustomMetadataCache.get_attr_id_for_name(
+            set_name=set_name, attr_name=attr_name
+        ):
+            return cls(field=attr_id)
+        else:
+            raise ValueError(
+                f"No custom metadata with the name {set_name} or property {attr_name} exists"
+            )
+
+    @classmethod
+    @validate_arguments()
     def with_categories(cls):
         return cls(field=TermAttributes.CATEGORIES.value)
 
     @classmethod
     @validate_arguments()
     def with_classification_names(cls):
         return cls(field=TextAttributes.CLASSIFICATION_NAMES.value)
@@ -322,14 +335,30 @@
     value: SearchFieldType
     boost: Optional[float] = None
     case_insensitive: Optional[bool] = None
     type_name: Literal["term"] = "term"
 
     @classmethod
     @validate_arguments()
+    def with_custom_metadata(
+        cls, set_name: StrictStr, attr_name: StrictStr, value: SearchFieldType
+    ):
+        from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+
+        if attr_id := CustomMetadataCache.get_attr_id_for_name(
+            set_name=set_name, attr_name=attr_name
+        ):
+            return cls(field=attr_id, value=value)
+        else:
+            raise ValueError(
+                f"No custom metadata with the name {set_name} or property {attr_name} exists"
+            )
+
+    @classmethod
+    @validate_arguments()
     def with_categories(cls, value: StrictStr):
         return cls(field=TermAttributes.CATEGORIES.value, value=value)
 
     @classmethod
     @validate_arguments()
     def with_connector_name(cls, value: AtlanConnectorType):
         return cls(field=TermAttributes.CONNECTOR_NAME.value, value=value.value)
```

### Comparing `pyatlan-0.0.31/pyatlan/model/structs.py` & `pyatlan-0.0.32/pyatlan/model/group.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,148 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
-from datetime import datetime
-from typing import Optional
+from __future__ import annotations
+
+from typing import List, Optional, Any
 
 from pydantic import Field
 
 from pyatlan.model.core import AtlanObject
-from pyatlan.model.enums import SourceCostUnitType
-
-
-class AwsTag(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        aws_tag_key: str = Field(None, description="", alias="awsTagKey")
-        aws_tag_value: str = Field(None, description="", alias="awsTagValue")
-
-
-class AwsCloudWatchMetric(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        aws_cloud_watch_metric_name: str = Field(
-            None, description="", alias="awsCloudWatchMetricName"
-        )
-        aws_cloud_watch_metric_scope: str = Field(
-            None, description="", alias="awsCloudWatchMetricScope"
-        )
-
-
-class Histogram(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        boundaries: set[float] = Field(None, description="", alias="boundaries")
-        frequencies: set[float] = Field(None, description="", alias="frequencies")
-
-
-class KafkaTopicConsumption(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        topic_name: Optional[str] = Field(None, description="", alias="topicName")
-        topic_partition: Optional[str] = Field(
-            None, description="", alias="topicPartition"
-        )
-        topic_lag: Optional[int] = Field(None, description="", alias="topicLag")
-        topic_current_offset: Optional[int] = Field(
-            None, description="", alias="topicCurrentOffset"
-        )
-
-
-class DbtMetricFilter(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        dbt_metric_filter_column_qualified_name: Optional[str] = Field(
-            None, description="", alias="dbtMetricFilterColumnQualifiedName"
-        )
-        dbt_metric_filter_field: Optional[str] = Field(
-            None, description="", alias="dbtMetricFilterField"
-        )
-        dbt_metric_filter_operator: Optional[str] = Field(
-            None, description="", alias="dbtMetricFilterOperator"
-        )
-        dbt_metric_filter_value: Optional[str] = Field(
-            None, description="", alias="dbtMetricFilterValue"
-        )
-
 
-class GoogleTag(AtlanObject):
-    """Description"""
 
+class AtlanGroup(AtlanObject):
     class Attributes(AtlanObject):
-        google_tag_key: str = Field(None, description="", alias="googleTagKey")
-        google_tag_value: str = Field(None, description="", alias="googleTagValue")
-
-
-class ColumnValueFrequencyMap(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        column_value: Optional[str] = Field(None, description="", alias="columnValue")
-        column_value_frequency: Optional[int] = Field(
-            None, description="", alias="columnValueFrequency"
-        )
-
-
-class BadgeCondition(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        badge_condition_operator: Optional[str] = Field(
-            None, description="", alias="badgeConditionOperator"
-        )
-        badge_condition_value: Optional[str] = Field(
-            None, description="", alias="badgeConditionValue"
-        )
-        badge_condition_colorhex: Optional[str] = Field(
-            None, description="", alias="badgeConditionColorhex"
-        )
-
-
-class AzureTag(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        azure_tag_key: str = Field(None, description="", alias="azureTagKey")
-        azure_tag_value: str = Field(None, description="", alias="azureTagValue")
-
-
-class GoogleLabel(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        google_label_key: str = Field(None, description="", alias="googleLabelKey")
-        google_label_value: str = Field(None, description="", alias="googleLabelValue")
-
-
-class PopularityInsights(AtlanObject):
-    """Description"""
-
-    class Attributes(AtlanObject):
-        record_user: Optional[str] = Field(None, description="", alias="recordUser")
-        record_query: Optional[str] = Field(None, description="", alias="recordQuery")
-        record_query_duration: Optional[int] = Field(
-            None, description="", alias="recordQueryDuration"
-        )
-        record_query_count: Optional[int] = Field(
-            None, description="", alias="recordQueryCount"
-        )
-        record_total_user_count: Optional[int] = Field(
-            None, description="", alias="recordTotalUserCount"
-        )
-        record_compute_cost: Optional[float] = Field(
-            None, description="", alias="recordComputeCost"
-        )
-        record_max_compute_cost: Optional[float] = Field(
-            None, description="", alias="recordMaxComputeCost"
-        )
-        record_compute_cost_unit: Optional[SourceCostUnitType] = Field(
-            None, description="", alias="recordComputeCostUnit"
-        )
-        record_last_timestamp: Optional[datetime] = Field(
-            None, description="", alias="recordLastTimestamp"
+        alias: Optional[List[str]] = Field(
+            description="Name of the group as it appears in the UI."
         )
-        record_warehouse: Optional[str] = Field(
-            None, description="", alias="recordWarehouse"
+        created_at: Optional[List[str]] = Field(
+            description="Time (epoch) at which the group was created, in milliseconds."
         )
+        created_by: Optional[List[str]] = Field(
+            description="User who created the group."
+        )
+        updated_at: Optional[List[str]] = Field(
+            description="Time (epoch) at which the group was last updated, in milliseconds."
+        )
+        updated_by: Optional[List[str]] = Field(
+            description="User who last updated the group."
+        )
+        description: Optional[List[str]] = Field(
+            description="Description of the group."
+        )
+        is_default: Optional[List[str]] = Field(
+            description="Whether this group should be auto-assigned to all new users or not."
+        )
+        channels: Optional[List[str]] = Field(
+            description="Slack channels for this group."
+        )
+
+    alias: Optional[str] = Field(
+        description="Name of the group as it appears in the UI."
+    )
+    attributes: Optional[AtlanGroup.Attributes] = Field(
+        description="Detailed attributes of the group."
+    )
+    decentralized_roles: Optional[str] = Field(description="TBC")
+    id: Optional[str] = Field(description="Unique identifier for the group (GUID).")
+    name: Optional[str] = Field(description="Unique (internal) name for the group.")
+    path: Optional[str] = Field(description="TBC")
+    personas: Optional[List[Any]] = Field(
+        description="Personas the group is associated with."
+    )
+    purposes: Optional[List[Any]] = Field(
+        description="Purposes the group is associated with."
+    )
+    user_count: Optional[int] = Field(description="Number of users in the group.")
+
+    def is_default(self) -> bool:
+        return (
+            self.attributes is not None
+            and self.attributes.is_default is not None
+            and self.attributes.is_default == "true"
+        )
+
+    @staticmethod
+    def create(
+        alias: str,
+    ) -> AtlanGroup:
+        from pyatlan.model.assets import validate_required_fields
+
+        validate_required_fields(
+            ["alias"],
+            [alias],
+        )
+        return AtlanGroup(
+            name=AtlanGroup.generate_name(alias),
+            attributes=AtlanGroup.Attributes(alias=[alias]),
+        )
+
+    @staticmethod
+    def create_for_modification(
+        guid: str,
+        path: str,
+    ) -> AtlanGroup:
+        from pyatlan.model.assets import validate_required_fields
+
+        validate_required_fields(
+            ["guid", "path"],
+            [guid, path],
+        )
+        return AtlanGroup(id=guid, path=path)
+
+    @staticmethod
+    def generate_name(
+        alias: str,
+    ) -> str:
+        from pyatlan.model.assets import validate_required_fields
+
+        validate_required_fields(
+            ["alias"],
+            [alias],
+        )
+        internal = alias.lower()
+        return internal.replace(" ", "_")
+
+
+class GroupResponse(AtlanObject):
+    total_record: Optional[int] = Field(description="Total number of groups.")
+    filter_record: Optional[int] = Field(
+        description="Number of groups in the filtered response.",
+    )
+    records: Optional[List[AtlanGroup]] = Field(
+        description="Details of each group included in the response."
+    )
+
+
+class CreateGroupRequest(AtlanObject):
+    group: AtlanGroup = Field(description="Group to be created.")
+    users: Optional[List[str]] = Field(
+        description="List of users (their GUIDs) to be included in the group."
+    )
+
+
+class RemoveFromGroupRequest(AtlanObject):
+    users: Optional[List[str]] = Field(
+        description="List of users (their GUIDs) to remove from the group."
+    )
+
+
+class CreateGroupResponse(AtlanObject):
+    class UserStatus(AtlanObject):
+        status: Optional[int] = Field(
+            description="Response code for the association (200 is success)."
+        )
+        status_message: Optional[str] = Field(
+            description="Status message for the association ('success' means the association was successful)."
+        )
+
+        def was_successful(self) -> bool:
+            return (self.status is not None and self.status == 200) or (
+                self.status_message is not None and self.status_message == "success"
+            )
+
+    group: str = Field(
+        description="Unique identifier (GUID) of the group that was created."
+    )
+    users: Optional[dict[str, CreateGroupResponse.UserStatus]] = Field(
+        description="Map of user association statuses, keyed by unique identifier (GUID) of the user."
+    )
```

### Comparing `pyatlan-0.0.31/pyatlan/utils.py` & `pyatlan-0.0.32/pyatlan/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 # Based on original code from https://github.com/apache/atlas (under Apache-2.0 license)
 import enum
 import logging
 import time
 from functools import reduce
-from typing import Optional
+from typing import Any, Optional
 
 ADMIN_URI = "api/service/"
 BASE_URI = "api/meta/"
 APPLICATION_JSON = "application/json"
 APPLICATION_OCTET_STREAM = "application/octet-stream"
 MULTIPART_FORM_DATA = "multipart/form-data"
 PREFIX_ATTR = "attr:"
@@ -104,14 +104,24 @@
     return (
         {k: type_coerce_list(v, obj_type) for k, v in obj.items()}
         if isinstance(obj, dict)
         else None
     )
 
 
+def validate_required_fields(field_names: list[str], values: list[Any]):
+    for field_name, value in zip(field_names, values):
+        if value is None:
+            raise ValueError(f"{field_name} is required")
+        if isinstance(value, str) and not value.strip():
+            raise ValueError(f"{field_name} cannot be blank")
+        if isinstance(value, list) and len(value) == 0:
+            raise ValueError(f"{field_name} cannot be an empty list")
+
+
 class API:
     def __init__(
         self,
         path,
         method,
         expected_status,
         consumes=APPLICATION_JSON,
```

### Comparing `pyatlan-0.0.31/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.0.32/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.0.31
+Version: 0.0.32
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.0.31/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.0.32/pyatlan.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,37 +13,43 @@
 pyatlan.egg-info/dependency_links.txt
 pyatlan.egg-info/not-zip-safe
 pyatlan.egg-info/requires.txt
 pyatlan.egg-info/top_level.txt
 pyatlan/cache/__init__.py
 pyatlan/cache/classification_cache.py
 pyatlan/cache/custom_metadata_cache.py
+pyatlan/cache/enum_cache.py
+pyatlan/cache/group_cache.py
 pyatlan/cache/role_cache.py
 pyatlan/client/__init__.py
 pyatlan/client/atlan.py
 pyatlan/client/constants.py
 pyatlan/generator/__init__.py
 pyatlan/generator/generate_from_typdefs.py
 pyatlan/generator/templates/__init__.py
 pyatlan/model/__init__.py
 pyatlan/model/assets.py
 pyatlan/model/core.py
 pyatlan/model/enums.py
+pyatlan/model/group.py
 pyatlan/model/internal.py
 pyatlan/model/lineage.py
 pyatlan/model/response.py
 pyatlan/model/role.py
 pyatlan/model/search.py
 pyatlan/model/structs.py
 pyatlan/model/typedef.py
 tests/__init__.py
+tests/conftest.py
 tests/integration/__init__.py
+tests/integration/admin_test.py
 tests/integration/classification_test.py
+tests/integration/client.py
 tests/integration/custom_metadata_test.py
-tests/integration/role_test.py
+tests/integration/glossary_test.py
 tests/integration/test_client.py
 tests/integration/test_entity_model.py
 tests/integration/test_index_search.py
 tests/unit/__init__.py
 tests/unit/test_classification_name.py
 tests/unit/test_client.py
 tests/unit/test_glossary_term.py
```

### Comparing `pyatlan-0.0.31/setup.py` & `pyatlan-0.0.32/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,16 @@
             "flake8>=5.0.4",
             "mypy>=0.991",
             "black>=22.10.0",
             "types-requests>=2.28.11.4",
             "pre-commit>=2.20.0",
             "deepdiff>=6.2.1",
             "pytest-cov>=4.0.0",
+            "pytest-order==1.1.0",
+            "retry==0.9.2",
             "twine>=4.0.2",
         ]
     },
     include_package_data=True,
     zip_safe=False,
     keywords="atlan client",
     python_requires=">=3.9",
```

### Comparing `pyatlan-0.0.31/tests/integration/test_client.py` & `pyatlan-0.0.32/tests/integration/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,65 +8,72 @@
 from pyatlan.model.enums import AtlanConnectorType
 from pyatlan.model.lineage import LineageRequest
 
 iter_count = count(1)
 
 
 @pytest.fixture(scope="module")
-def client() -> AtlanClient:
-    return AtlanClient()
+def m_client() -> AtlanClient:
+    from os import environ
+
+    client = AtlanClient(
+        base_url=environ["MARK_BASE_URL"], api_key=environ["MARK_API_KEY"]
+    )
+    AtlanClient.register_client(client)
+    return client
 
 
 @pytest.fixture(scope="module")
-def connection(client: AtlanClient) -> Connection:
-    return client.get_asset_by_guid("b3a5c49a-0c7c-4e66-8453-f4da8d9ce222", Connection)
+def connection(m_client) -> Connection:
+    return m_client.get_asset_by_guid(
+        "b3a5c49a-0c7c-4e66-8453-f4da8d9ce222", Connection
+    )
 
 
 @pytest.fixture(scope="module")
-def glossary(client: AtlanClient) -> Generator[AtlasGlossary, None, None]:
+def glossary(m_client: AtlanClient) -> Generator[AtlasGlossary, None, None]:
     glossary = AtlasGlossary.create(name="Integration Test Glossary")
-    glossary = client.upsert(glossary).assets_created(asset_type=AtlasGlossary)[0]
+    glossary = m_client.upsert(glossary).assets_created(asset_type=AtlasGlossary)[0]
     yield glossary
-    client.purge_entity_by_guid(guid=glossary.guid)
+    m_client.purge_entity_by_guid(guid=glossary.guid)
 
 
 @pytest.fixture()
 def database(
-    client: AtlanClient, connection: Connection
+    m_client: AtlanClient, connection: Connection
 ) -> Generator[Database, None, None]:
-
     database = Database.create(
         name=f"Integration_Test_Entity_DB{next(iter_count)}",
         connection_qualified_name=connection.attributes.qualified_name,
     )
-    database = client.upsert(database).assets_created(Database)[0]
+    database = m_client.upsert(database).assets_created(Database)[0]
 
     yield database
 
-    client.purge_entity_by_guid(guid=database.guid)
+    m_client.purge_entity_by_guid(guid=database.guid)
 
 
 @pytest.fixture()
 def make_term(
-    client: AtlanClient, glossary
+    m_client: AtlanClient, glossary
 ) -> Generator[Callable[[str], AtlasGlossaryTerm], None, None]:
     created_term_guids = []
 
     def _make_term(name: str) -> AtlasGlossaryTerm:
         term = AtlasGlossaryTerm.create(
             name=f"Integration Test Glossary Term {name}", anchor=glossary
         )
-        term = client.upsert(term).assets_created(AtlasGlossaryTerm)[0]
+        term = m_client.upsert(term).assets_created(AtlasGlossaryTerm)[0]
         created_term_guids.append(term.guid)
         return term
 
     yield _make_term
 
     for guid in created_term_guids:
-        client.purge_entity_by_guid(guid=guid)
+        m_client.purge_entity_by_guid(guid=guid)
 
 
 def test_register_client_with_bad_parameter_raises_valueerror():
     with pytest.raises(ValueError, match="client must be an instance of AtlanClient"):
         AtlanClient.register_client("")
     assert AtlanClient.get_default_client() is None
 
@@ -74,168 +81,168 @@
 def test_register_client():
     client = AtlanClient(base_url="http://mark.atlan.com", api_key="123")
     AtlanClient.register_client(client)
     assert AtlanClient.get_default_client() == client
 
 
 def test_append_terms_with_guid(
-    client: AtlanClient,
+    m_client: AtlanClient,
     make_term: Callable[[str], AtlasGlossaryTerm],
     database: Database,
 ):
     term = make_term("Term1")
 
     assert (
-        database := client.append_terms(
+        database := m_client.append_terms(
             guid=database.guid, asset_type=Database, terms=[term]
         )
     )
-    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert len(database.terms) == 1
     assert database.terms[0].guid == term.guid
 
 
 def test_append_terms_with_qualified_name(
-    client: AtlanClient,
+    m_client: AtlanClient,
     make_term: Callable[[str], AtlasGlossaryTerm],
     database: Database,
 ):
     term = make_term("Term1")
 
     assert (
-        database := client.append_terms(
+        database := m_client.append_terms(
             qualified_name=database.qualified_name, asset_type=Database, terms=[term]
         )
     )
-    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert len(database.terms) == 1
     assert database.terms[0].guid == term.guid
 
 
 def test_append_terms_using_ref_by_guid_for_term(
-    client: AtlanClient,
+    m_client: AtlanClient,
     make_term: Callable[[str], AtlasGlossaryTerm],
     database: Database,
 ):
     term = make_term("Term1")
 
     assert (
-        database := client.append_terms(
+        database := m_client.append_terms(
             qualified_name=database.qualified_name,
             asset_type=Database,
             terms=[AtlasGlossaryTerm.ref_by_guid(guid=term.guid)],
         )
     )
-    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert len(database.terms) == 1
     assert database.terms[0].guid == term.guid
 
 
 def test_replace_a_term(
-    client: AtlanClient,
+    m_client: AtlanClient,
     make_term: Callable[[str], AtlasGlossaryTerm],
     database: Database,
 ):
     original_term = make_term("Term1")
     assert (
-        database := client.append_terms(
+        database := m_client.append_terms(
             qualified_name=database.qualified_name,
             asset_type=Database,
             terms=[AtlasGlossaryTerm.ref_by_guid(guid=original_term.guid)],
         )
     )
 
     replacemant_term = make_term("Term2")
     assert (
-        database := client.replace_terms(
+        database := m_client.replace_terms(
             guid=database.guid, asset_type=Database, terms=[replacemant_term]
         )
     )
 
-    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert len(database.terms) == 2
     deleted_terms = [t for t in database.terms if t.relationship_status == "DELETED"]
     assert len(deleted_terms) == 1
     assert deleted_terms[0].guid == original_term.guid
     active_terms = [t for t in database.terms if t.relationship_status != "DELETED"]
     assert len(active_terms) == 1
     assert active_terms[0].guid == replacemant_term.guid
 
 
 def test_replace_all_term(
-    client: AtlanClient,
+    m_client: AtlanClient,
     make_term: Callable[[str], AtlasGlossaryTerm],
     database: Database,
 ):
     original_term = make_term("Term1")
     assert (
-        database := client.append_terms(
+        database := m_client.append_terms(
             qualified_name=database.qualified_name,
             asset_type=Database,
             terms=[AtlasGlossaryTerm.ref_by_guid(guid=original_term.guid)],
         )
     )
 
     assert (
-        database := client.replace_terms(
+        database := m_client.replace_terms(
             guid=database.guid, asset_type=Database, terms=[]
         )
     )
 
-    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert len(database.terms) == 1
     deleted_terms = [t for t in database.terms if t.relationship_status == "DELETED"]
     assert len(deleted_terms) == 1
     assert deleted_terms[0].guid == original_term.guid
 
 
 def test_remove_term(
-    client: AtlanClient,
+    m_client: AtlanClient,
     make_term: Callable[[str], AtlasGlossaryTerm],
     database: Database,
 ):
     original_term = make_term("Term1")
     another_term = make_term("Term2")
     assert (
-        database := client.append_terms(
+        database := m_client.append_terms(
             qualified_name=database.qualified_name,
             asset_type=Database,
             terms=[
                 AtlasGlossaryTerm.ref_by_guid(guid=original_term.guid),
                 AtlasGlossaryTerm.ref_by_guid(guid=another_term.guid),
             ],
         )
     )
 
     assert (
-        database := client.remove_terms(
+        database := m_client.remove_terms(
             guid=database.guid,
             asset_type=Database,
             terms=[AtlasGlossaryTerm.ref_by_guid(original_term.guid)],
         )
     )
 
-    database = client.get_asset_by_guid(guid=database.guid, asset_type=Database)
+    database = m_client.get_asset_by_guid(guid=database.guid, asset_type=Database)
     assert len(database.terms) == 2
     deleted_terms = [t for t in database.terms if t.relationship_status == "DELETED"]
     assert len(deleted_terms) == 1
     assert deleted_terms[0].guid == original_term.guid
     active_terms = [t for t in database.terms if t.relationship_status != "DELETED"]
     assert active_terms[0].guid == another_term.guid
 
 
-def test_find_connections_by_name(client: AtlanClient):
-    connections = client.find_connections_by_name(
+def test_find_connections_by_name(m_client: AtlanClient):
+    connections = m_client.find_connections_by_name(
         name="Test Connection",
         connector_type=AtlanConnectorType.SNOWFLAKE,
         attributes=["connectorName"],
     )
     assert len(connections) == 1
     assert connections[0].connector_name == AtlanConnectorType.SNOWFLAKE.value
 
 
-def test_get_lineage(client: AtlanClient):
-    response = client.get_lineage(
+def test_get_lineage(m_client: AtlanClient):
+    response = m_client.get_lineage(
         LineageRequest(guid="75474eab-3105-4ef9-9f84-709e386a7d3e")
     )
     for guid, asset in response.guid_entity_map.items():
         assert guid == asset.guid
```

### Comparing `pyatlan-0.0.31/tests/integration/test_entity_model.py` & `pyatlan-0.0.32/tests/integration/test_entity_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,16 +46,22 @@
     "57f5463d-cc2a-4859-bf28-e4fa52002e8e",
 }
 TEMP_CONNECTION_GUID = "b3a5c49a-0c7c-4e66-8453-f4da8d9ce222"
 S3_CONNECTION_GUID = "25f2dc21-cd53-47fe-bbed-be10759d087a"
 
 
 @pytest.fixture(scope="module")
-def client() -> AtlanClient:
-    return AtlanClient()
+def m_client() -> AtlanClient:
+    from os import environ
+
+    client = AtlanClient(
+        base_url=environ["MARK_BASE_URL"], api_key=environ["MARK_API_KEY"]
+    )
+    AtlanClient.register_client(client)
+    return client
 
 
 @pytest.fixture()
 def announcement() -> Announcement:
     return Announcement(
         announcement_title="Important Announcement",
         announcement_message="A message".join(
@@ -63,20 +69,20 @@
         ),
         announcement_type=AnnouncementType.ISSUE,
     )
 
 
 @pytest.fixture(scope="session")
 def atlan_host() -> str:
-    return get_environment_variable("ATLAN_BASE_URL")
+    return get_environment_variable("MARK_BASE_URL")
 
 
 @pytest.fixture(scope="session")
 def atlan_api_key() -> str:
-    return get_environment_variable("ATLAN_API_KEY")
+    return get_environment_variable("MARK_API_KEY")
 
 
 @pytest.fixture(scope="session")
 def headers(atlan_api_key):
     return {
         "accept": "application/json, text/plain, */*",
         "content-type": "application/json",
@@ -200,678 +206,686 @@
         print()
         delete_assets(atlan_host, headers, type_name)
     yield
     for type_name in type_names:
         delete_assets(atlan_host, headers, type_name)
 
 
-def test_get_glossary_by_guid_good_guid(create_glossary, client: AtlanClient):
-    glossary = client.get_asset_by_guid(create_glossary(), AtlasGlossary)
+def test_get_glossary_by_guid_good_guid(create_glossary, m_client: AtlanClient):
+    glossary = m_client.get_asset_by_guid(create_glossary(), AtlasGlossary)
     assert isinstance(glossary, AtlasGlossary)
 
 
 def test_get_asset_by_guid_when_table_specified_and_glossary_returned_raises_not_found_error(
-    create_glossary, client: AtlanClient
+    create_glossary, m_client: AtlanClient
 ):
     with pytest.raises(NotFoundError) as ex_info:
         guid = create_glossary()
-        client.get_asset_by_guid(guid, Table)
+        m_client.get_asset_by_guid(guid, Table)
     assert (
         f"Asset with GUID {guid} is not of the type requested: Table."
         in ex_info.value.args[0]
     )
 
 
-def test_get_glossary_by_guid_bad_guid(client: AtlanClient):
+def test_get_glossary_by_guid_bad_guid(m_client: AtlanClient):
     with pytest.raises(NotFoundError) as ex_info:
-        client.get_asset_by_guid("76d54dd6-925b-499b-a455-6", AtlasGlossary)
+        m_client.get_asset_by_guid("76d54dd6-925b-499b-a455-6", AtlasGlossary)
     assert (
         "Given instance guid 76d54dd6-925b-499b-a455-6 is invalid/not found"
         in ex_info.value.args[0]
     )
 
 
-def test_update_glossary_when_no_changes(create_glossary, client: AtlanClient):
-    glossary = client.get_asset_by_guid(create_glossary(), AtlasGlossary)
-    response = client.upsert(glossary)
+def test_update_glossary_when_no_changes(create_glossary, m_client: AtlanClient):
+    glossary = m_client.get_asset_by_guid(create_glossary(), AtlasGlossary)
+    response = m_client.upsert(glossary)
     assert not response.guid_assignments
     assert not response.mutated_entities
 
 
 def test_update_glossary_with_changes(
-    create_glossary, client: AtlanClient, announcement
+    create_glossary, m_client: AtlanClient, announcement
 ):
-    glossary = client.get_asset_by_guid(create_glossary(), AtlasGlossary)
+    glossary = m_client.get_asset_by_guid(create_glossary(), AtlasGlossary)
     glossary.set_announcement(announcement)
-    response = client.upsert(glossary)
+    response = m_client.upsert(glossary)
     assert not response.guid_assignments
     assert response.mutated_entities
     assert not response.mutated_entities.CREATE
     assert not response.mutated_entities.DELETE
     assert response.mutated_entities.UPDATE
     assert len(response.mutated_entities.UPDATE) == 1
     assert isinstance(response.mutated_entities.UPDATE[0], AtlasGlossary)
     glossary = response.mutated_entities.UPDATE[0]
     assert glossary.attributes.announcement_title == announcement.announcement_title
 
 
-def test_purge_glossary(create_glossary, client: AtlanClient):
-    response = client.purge_entity_by_guid(create_glossary())
+def test_purge_glossary(create_glossary, m_client: AtlanClient):
+    response = m_client.purge_entity_by_guid(create_glossary())
     assert response.mutated_entities
     assert response.mutated_entities.DELETE
     assert len(response.mutated_entities.DELETE) == 1
     assert not response.mutated_entities.UPDATE
     assert not response.mutated_entities.CREATE
 
 
-def test_create_glossary(client: AtlanClient, increment_counter):
+def test_create_glossary(m_client: AtlanClient, increment_counter):
     glossary = AtlasGlossary.create(
         name=f"Integration Test Glossary {increment_counter()}"
     )
-    response = client.upsert(glossary)
+    response = m_client.upsert(glossary)
     assert response.mutated_entities
     assert not response.mutated_entities.UPDATE
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     guid = list(response.guid_assignments.values())[0]
     assert response.mutated_entities.CREATE
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossary)
     glossary = response.mutated_entities.CREATE[0]
     assert glossary.guid == guid
 
 
-def test_create_multiple_glossaries_one_at_time(client: AtlanClient, increment_counter):
+def test_create_multiple_glossaries_one_at_time(
+    m_client: AtlanClient, increment_counter
+):
     glossary = AtlasGlossary(
         attributes=AtlasGlossary.Attributes(
             name=f"Integration Test Glossary {increment_counter()}",
             user_description="This a test glossary",
         )
     )
-    response = client.upsert(glossary)
+    response = m_client.upsert(glossary)
     assert response.mutated_entities
     assert not response.mutated_entities.UPDATE
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     guid = list(response.guid_assignments.values())[0]
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossary)
     glossary = response.mutated_entities.CREATE[0]
     assert glossary.guid == guid
     glossary = AtlasGlossary(
         attributes=AtlasGlossary.Attributes(
             name=f"Integration Test Glossary {increment_counter()}",
             user_description="This a test glossary",
         )
     )
-    response = client.upsert(glossary)
+    response = m_client.upsert(glossary)
     assert response.mutated_entities
     assert not response.mutated_entities.UPDATE
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     guid = list(response.guid_assignments.values())[0]
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossary)
     glossary = response.mutated_entities.CREATE[0]
     assert glossary.guid == guid
 
 
-def test_create_multiple_glossaries(client: AtlanClient, increment_counter):
+def test_create_multiple_glossaries(m_client: AtlanClient, increment_counter):
     entities: list[Asset] = []
     count = 2
     for i in range(count):
         entities.append(
             AtlasGlossary.create(
                 name=f"Integration Test Glossary {increment_counter() + i}"
             )
         )
-    response = client.upsert(entities)
+    response = m_client.upsert(entities)
     assert response.mutated_entities
     assert not response.mutated_entities.UPDATE
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == count
     for glossary in response.assets_created(AtlasGlossary):
         assert glossary.guid in response.guid_assignments.values()
 
 
-def test_create_glossary_category(client: AtlanClient, increment_counter):
+def test_create_glossary_category(m_client: AtlanClient, increment_counter):
     suffix = increment_counter()
     glossary = AtlasGlossary.create(name=f"Integration Test Glossary {suffix}")
     glossary.attributes.user_description = "This a test glossary"
-    response = client.upsert(glossary)
+    response = m_client.upsert(glossary)
     assert response.mutated_entities
     assert response.mutated_entities.CREATE
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossary)
     glossary = response.mutated_entities.CREATE[0]
     category = AtlasGlossaryCategory.create(
         name=f"Integration Test Glossary Category {suffix}", anchor=glossary
     )
     category.attributes.user_description = "This is a test glossary category"
-    response = client.upsert(category)
+    response = m_client.upsert(category)
     assert response.mutated_entities
     assert response.mutated_entities.UPDATE
     assert len(response.mutated_entities.UPDATE) == 1
     assert isinstance(response.mutated_entities.UPDATE[0], AtlasGlossary)
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     guid = list(response.guid_assignments.values())[0]
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossaryCategory)
     category = response.mutated_entities.CREATE[0]
     assert isinstance(category, AtlasGlossaryCategory)
     assert guid == category.guid
-    category = client.get_asset_by_guid(guid, AtlasGlossaryCategory)
+    category = m_client.get_asset_by_guid(guid, AtlasGlossaryCategory)
     assert isinstance(category, AtlasGlossaryCategory)
     assert category.guid == guid
 
 
-def test_create_glossary_term(client: AtlanClient, increment_counter):
+def test_create_glossary_term(m_client: AtlanClient, increment_counter):
     suffix = increment_counter()
     glossary = AtlasGlossary.create(name=f"Integration Test Glossary {suffix}")
-    response = client.upsert(glossary)
+    response = m_client.upsert(glossary)
     assert response.mutated_entities
     assert response.mutated_entities.CREATE
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossary)
     glossary = response.mutated_entities.CREATE[0]
     term = AtlasGlossaryTerm.create(
         name=f"Integration Test Glossary Term {suffix}", anchor=glossary
     )
-    response = client.upsert(term)
+    response = m_client.upsert(term)
     assert response.mutated_entities
     assert response.mutated_entities.UPDATE
     assert response.mutated_entities.UPDATE
     assert len(response.mutated_entities.UPDATE) == 1
     assert isinstance(response.mutated_entities.UPDATE[0], AtlasGlossary)
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     guid = list(response.guid_assignments.values())[0]
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossaryTerm)
     term = response.mutated_entities.CREATE[0]
     assert guid == term.guid
-    term = client.get_asset_by_guid(guid, AtlasGlossaryTerm)
+    term = m_client.get_asset_by_guid(guid, AtlasGlossaryTerm)
     assert isinstance(term, AtlasGlossaryTerm)
     assert term.guid == guid
 
     term = AtlasGlossaryTerm.create_for_modification(
         qualified_name=term.qualified_name,
         name=term.name,
         glossary_guid=glossary.guid,
     )
     term.user_description = "This is an important term"
-    response = client.upsert(term)
+    response = m_client.upsert(term)
     assert 1 == len(response.assets_updated(AtlasGlossaryTerm))
 
 
 def test_create_glossary_term_with_glossary_guid(
-    client: AtlanClient, increment_counter
+    m_client: AtlanClient, increment_counter
 ):
     suffix = increment_counter()
     glossary = AtlasGlossary.create(name=f"Integration Test Glossary {suffix}")
-    response = client.upsert(glossary)
+    response = m_client.upsert(glossary)
     assert response.mutated_entities
     assert response.mutated_entities.CREATE
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossary)
     glossary = response.mutated_entities.CREATE[0]
     term = AtlasGlossaryTerm.create(
         name=f"Integration Test Glossary Term {suffix}", glossary_guid=glossary.guid
     )
-    response = client.upsert(term)
+    response = m_client.upsert(term)
     assert response.mutated_entities
     assert response.mutated_entities.UPDATE
     assert response.mutated_entities.UPDATE
     assert len(response.mutated_entities.UPDATE) == 1
     assert isinstance(response.mutated_entities.UPDATE[0], AtlasGlossary)
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     guid = list(response.guid_assignments.values())[0]
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossaryTerm)
     term = response.mutated_entities.CREATE[0]
     assert guid == term.guid
-    term = client.get_asset_by_guid(guid, AtlasGlossaryTerm)
+    term = m_client.get_asset_by_guid(guid, AtlasGlossaryTerm)
     assert isinstance(term, AtlasGlossaryTerm)
     assert term.guid == guid
 
 
 def test_create_glossary_term_with_glossary_qualified_name(
-    client: AtlanClient, increment_counter
+    m_client: AtlanClient, increment_counter
 ):
     suffix = increment_counter()
     glossary = AtlasGlossary.create(name=f"Integration Test Glossary {suffix}")
-    response = client.upsert(glossary)
+    response = m_client.upsert(glossary)
     assert response.mutated_entities
     assert response.mutated_entities.CREATE
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossary)
     glossary = response.mutated_entities.CREATE[0]
     term = AtlasGlossaryTerm.create(
         name=f"Integration Test Glossary Term {suffix}",
         glossary_qualified_name=glossary.qualified_name,
     )
-    response = client.upsert(term)
+    response = m_client.upsert(term)
     assert response.mutated_entities
     assert response.mutated_entities.UPDATE
     assert response.mutated_entities.UPDATE
     assert len(response.mutated_entities.UPDATE) == 1
     assert isinstance(response.mutated_entities.UPDATE[0], AtlasGlossary)
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     guid = list(response.guid_assignments.values())[0]
     assert isinstance(response.mutated_entities.CREATE[0], AtlasGlossaryTerm)
     term = response.mutated_entities.CREATE[0]
     assert guid == term.guid
-    term = client.get_asset_by_guid(guid, AtlasGlossaryTerm)
+    term = m_client.get_asset_by_guid(guid, AtlasGlossaryTerm)
     assert isinstance(term, AtlasGlossaryTerm)
     assert term.guid == guid
 
 
-def test_create_hierarchy(client: AtlanClient, increment_counter):
+def test_create_hierarchy(m_client: AtlanClient, increment_counter):
     suffix = increment_counter()
     glossary = AtlasGlossary(
         attributes=AtlasGlossary.Attributes(
             name=f"Integration Test Glossary {suffix}",
             user_description="This a test glossary",
         )
     )
-    response = client.upsert(glossary)
+    response = m_client.upsert(glossary)
     assert len(response.assets_created(AtlasGlossary)) == 1
     glossary = response.assets_created(AtlasGlossary)[0]
     category_1 = AtlasGlossaryCategory(
         attributes=AtlasGlossaryCategory.Attributes(
             name=f"Integration Test Glossary Category {suffix}",
             user_description="This is a test glossary category",
             anchor=glossary,
         )
     )
-    response = client.upsert(category_1)
+    response = m_client.upsert(category_1)
     assert len(response.assets_updated(AtlasGlossary)) == 1
     assert len(response.assets_created(AtlasGlossaryCategory)) == 1
     guid = list(response.guid_assignments.values())[0]
     category_1 = response.assets_created(AtlasGlossaryCategory)[0]
     assert guid == category_1.guid
     category_2 = AtlasGlossaryCategory.create(
         name=f"Integration Test Glossary Category {suffix}",
         anchor=glossary,
         parent_category=category_1,
     )
-    response = client.upsert(category_2)
+    response = m_client.upsert(category_2)
     guid = list(response.guid_assignments.values())[0]
     assert len(response.assets_updated(AtlasGlossary)) == 1
     assert len(response.assets_updated(AtlasGlossaryCategory)) == 1
     assert len(response.assets_created(AtlasGlossaryCategory)) == 1
     category_2 = response.assets_created(AtlasGlossaryCategory)[0]
     assert guid == category_2.guid
     term = AtlasGlossaryTerm.create(
         name=f"Integration Test term {suffix}", anchor=glossary, categories=[category_2]
     )
-    response = client.upsert(term)
+    response = m_client.upsert(term)
     assert len(response.assets_updated(AtlasGlossary)) == 1
     assert len(response.assets_updated(AtlasGlossaryCategory)) == 1
     guid = list(response.guid_assignments.values())[0]
     assert len(response.assets_created(AtlasGlossaryTerm)) == 1
     term = response.assets_created(AtlasGlossaryTerm)[0]
     assert guid == term.guid
 
 
 @pytest.mark.skip("Connection creation is still intermittently failing")
-def test_create_connection(client: AtlanClient, increment_counter):
+def test_create_connection(m_client: AtlanClient, increment_counter):
     role = RoleCache.get_id_for_name("$admin")
     assert role
     c = Connection.create(
         name=f"Integration {increment_counter()}",
         connector_type=AtlanConnectorType.SNOWFLAKE,
         admin_roles=[role],
         admin_groups=["admin"],
     )
-    response = client.upsert(c)
+    response = m_client.upsert(c)
     assert response.mutated_entities
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     assert isinstance(response.mutated_entities.CREATE[0], Connection)
     assert response.guid_assignments
     assert c.guid in response.guid_assignments
     guid = response.guid_assignments[c.guid]
     c = response.mutated_entities.CREATE[0]
     assert guid == c.guid
-    c = client.get_asset_by_guid(c.guid, Connection)
+    c = m_client.get_asset_by_guid(c.guid, Connection)
     assert isinstance(c, Connection)
     assert c.guid == guid
 
 
-def test_create_database(client: AtlanClient, increment_counter):
+def test_create_database(m_client: AtlanClient, increment_counter):
     role = RoleCache.get_id_for_name("$admin")
     assert role
     suffix = increment_counter()
     # connection = Connection.create(
     #     name=f"Integration {suffix}",
     #     connector_type=AtlanConnectorType.SNOWFLAKE,
     #     admin_roles=[role],
     #     admin_groups=["admin"],
     # )
-    # response = client.upsert(connection)
+    # response = m_client.upsert(connection)
     # assert response.mutated_entities
     # assert response.mutated_entities.CREATE
     # assert isinstance(response.mutated_entities.CREATE[0], Connection)
     # connection = response.mutated_entities.CREATE[0]
-    # connection = client.get_asset_by_guid(connection.guid, Connection)
-    connection = client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
+    # connection = m_client.get_asset_by_guid(connection.guid, Connection)
+    connection = m_client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
     database = Database.create(
         name=f"Integration_{suffix}",
         connection_qualified_name=connection.attributes.qualified_name,
     )
-    response = client.upsert(database)
+    response = m_client.upsert(database)
     assert response.mutated_entities
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     assert isinstance(response.mutated_entities.CREATE[0], Database)
     assert response.guid_assignments
     database = response.mutated_entities.CREATE[0]
-    client.get_asset_by_guid(database.guid, Database)
+    m_client.get_asset_by_guid(database.guid, Database)
 
 
-def test_create_schema(client: AtlanClient, increment_counter):
+def test_create_schema(m_client: AtlanClient, increment_counter):
     role = RoleCache.get_id_for_name("$admin")
     assert role
     suffix = increment_counter()
     # connection = Connection.create(
     #     name=f"Integration {suffix}",
     #     connector_type=AtlanConnectorType.SNOWFLAKE,
     #     admin_roles=[role],
     #     admin_groups=["admin"],
     # )
-    # response = client.upsert(connection)
+    # response = m_client.upsert(connection)
     # assert response.mutated_entities
     # assert response.mutated_entities.CREATE
     # assert isinstance(response.mutated_entities.CREATE[0], Connection)
     # connection = response.mutated_entities.CREATE[0]
     # time.sleep(30)
-    connection = client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
+    connection = m_client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
     database = Database.create(
         name=f"Integration_{suffix}",
         connection_qualified_name=connection.attributes.qualified_name,
     )
-    response = client.upsert(database)
+    response = m_client.upsert(database)
     assert (databases := response.assets_created(asset_type=Database))
     assert len(databases) == 1
-    database = client.get_asset_by_guid(databases[0].guid, Database)
+    database = m_client.get_asset_by_guid(databases[0].guid, Database)
     schema = Schema.create(
         name=f"Integration_{suffix}",
         database_qualified_name=database.attributes.qualified_name,
     )
-    response = client.upsert(schema)
+    response = m_client.upsert(schema)
     assert (schemas := response.assets_created(asset_type=Schema))
     assert len(schemas) == 1
-    schema = client.get_asset_by_guid(schemas[0].guid, Schema)
+    schema = m_client.get_asset_by_guid(schemas[0].guid, Schema)
     assert (databases := response.assets_updated(asset_type=Database))
     assert len(databases) == 1
-    database = client.get_asset_by_guid(databases[0].guid, Database)
+    database = m_client.get_asset_by_guid(databases[0].guid, Database)
     assert database.attributes.schemas
     schemas = database.attributes.schemas
     assert len(schemas) == 1
     assert schemas[0].guid == schema.guid
 
 
-def test_create_table(client: AtlanClient, increment_counter):
+def test_create_table(m_client: AtlanClient, increment_counter):
     role = RoleCache.get_id_for_name("$admin")
     assert role
     suffix = increment_counter()
     # connection = Connection.create(
     #     name=f"Integration {suffix}",
     #     connector_type=AtlanConnectorType.SNOWFLAKE,
     #     admin_roles=[role],
     #     admin_groups=["admin"],
     # )
-    # response = client.upsert(connection)
+    # response = m_client.upsert(connection)
     # assert response.mutated_entities
     # assert response.mutated_entities.CREATE
     # assert isinstance(response.mutated_entities.CREATE[0], Connection)
     # connection = response.mutated_entities.CREATE[0]
     # time.sleep(30)
-    connection = client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
+    connection = m_client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
     database = Database.create(
         name=f"Integration_{suffix}",
         connection_qualified_name=connection.attributes.qualified_name,
     )
-    response = client.upsert(database)
+    response = m_client.upsert(database)
     assert (databases := response.assets_created(asset_type=Database))
-    database = client.get_asset_by_guid(databases[0].guid, Database)
+    database = m_client.get_asset_by_guid(databases[0].guid, Database)
     schema = Schema.create(
         name=f"Integration_{suffix}",
         database_qualified_name=database.attributes.qualified_name,
     )
-    response = client.upsert(schema)
+    response = m_client.upsert(schema)
     assert (schemas := response.assets_created(asset_type=Schema))
-    schema = client.get_asset_by_guid(schemas[0].guid, Schema)
+    schema = m_client.get_asset_by_guid(schemas[0].guid, Schema)
     table = Table.create(
         name=f"Integration_{suffix}",
         schema_qualified_name=schema.attributes.qualified_name,
     )
-    response = client.upsert(table)
+    response = m_client.upsert(table)
     assert (tables := response.assets_created(asset_type=Table))
     assert len(tables) == 1
-    table = client.get_asset_by_guid(guid=tables[0].guid, asset_type=Table)
+    table = m_client.get_asset_by_guid(guid=tables[0].guid, asset_type=Table)
     assert (schemas := response.assets_updated(asset_type=Schema))
     assert len(schemas) == 1
-    schema = client.get_asset_by_guid(guid=schemas[0].guid, asset_type=Schema)
+    schema = m_client.get_asset_by_guid(guid=schemas[0].guid, asset_type=Schema)
     assert schema.attributes.tables
     tables = schema.attributes.tables
     assert len(tables) == 1
     assert tables[0].guid == table.guid
 
 
-def test_get_by_qualified_name(client: AtlanClient):
+def test_get_by_qualified_name(m_client: AtlanClient):
     qualified_name = "default/snowflake/1646836521/ATLAN_SAMPLE_DATA/DBT_SARORA/RAW_CUSTOMERS/LAST_NAME"
-    column = client.get_asset_by_qualified_name(
+    column = m_client.get_asset_by_qualified_name(
         qualified_name=qualified_name, asset_type=Column
     )
     assert column.attributes.qualified_name == qualified_name
 
 
 @pytest.mark.skip("Connection creation is still intermittently failing")
-def test_create_view(client: AtlanClient, increment_counter):
+def test_create_view(m_client: AtlanClient, increment_counter):
     view = View.create(
         name=f"Integration {increment_counter()}",
         schema_qualified_name="default/snowflake/1658945299/ATLAN_SAMPLE_DATA/US_ECONOMIC_DATA",
     )
-    response = client.upsert(view)
+    response = m_client.upsert(view)
     assert response.mutated_entities
     assert response.mutated_entities.CREATE
     assert len(response.mutated_entities.CREATE) == 1
     assert isinstance(response.mutated_entities.CREATE[0], View)
     assert response.guid_assignments
     assert view.guid in response.guid_assignments
     guid = response.guid_assignments[view.guid]
     view = response.mutated_entities.CREATE[0]
     assert guid == view.guid
 
 
-def test_create_column(client: AtlanClient, increment_counter):
+def test_create_column(m_client: AtlanClient, increment_counter):
     role = RoleCache.get_id_for_name("$admin")
     assert role
     suffix = increment_counter()
     # connection = Connection.create(
     #     name=f"Integration {suffix}",
     #     connector_type=AtlanConnectorType.SNOWFLAKE,
     #     admin_roles=[role],
     #     admin_groups=["admin"],
     # )
-    # response = client.upsert(connection)
+    # response = m_client.upsert(connection)
     # assert response.mutated_entities
     # assert response.mutated_entities.CREATE
     # assert isinstance(response.mutated_entities.CREATE[0], Connection)
     # connection = response.mutated_entities.CREATE[0]
     # time.sleep(30)
-    connection = client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
+    connection = m_client.get_asset_by_guid(TEMP_CONNECTION_GUID, Connection)
     database = Database.create(
         name=f"Integration_{suffix}",
         connection_qualified_name=connection.attributes.qualified_name,
     )
-    response = client.upsert(database)
+    response = m_client.upsert(database)
     assert (databases := response.assets_created(asset_type=Database))
-    database = client.get_asset_by_guid(databases[0].guid, Database)
+    database = m_client.get_asset_by_guid(databases[0].guid, Database)
     schema = Schema.create(
         name=f"Integration_{suffix}",
         database_qualified_name=database.attributes.qualified_name,
     )
-    response = client.upsert(schema)
+    response = m_client.upsert(schema)
     assert (schemas := response.assets_created(asset_type=Schema))
-    schema = client.get_asset_by_guid(schemas[0].guid, Schema)
+    schema = m_client.get_asset_by_guid(schemas[0].guid, Schema)
     table = Table.create(
         name=f"Integration_{suffix}",
         schema_qualified_name=schema.attributes.qualified_name,
     )
-    response = client.upsert(table)
+    response = m_client.upsert(table)
     assert (tables := response.assets_created(asset_type=Table))
-    table = client.get_asset_by_guid(guid=tables[0].guid, asset_type=Table)
+    table = m_client.get_asset_by_guid(guid=tables[0].guid, asset_type=Table)
     column = Column.create(
         name=f"Integration_{suffix}_column",
         parent_qualified_name=table.qualified_name,
         parent_type=Table,
         order=1,
     )
-    response = client.upsert(column)
+    response = m_client.upsert(column)
     assert (columns := response.assets_created(asset_type=Column))
     assert len(columns) == 1
-    column = client.get_asset_by_guid(asset_type=Column, guid=columns[0].guid)
-    table = client.get_asset_by_guid(asset_type=Table, guid=table.guid)
+    column = m_client.get_asset_by_guid(asset_type=Column, guid=columns[0].guid)
+    table = m_client.get_asset_by_guid(asset_type=Table, guid=table.guid)
     assert table.attributes.columns
     columns = table.attributes.columns
     assert len(columns) == 1
     assert columns[0].guid == column.guid
 
 
-def test_add_and_remove_classifications(client: AtlanClient):
+def test_add_and_remove_classifications(m_client: AtlanClient):
     glossary = AtlasGlossary.create(name="Integration Classification Test")
     glossary.attributes.user_description = "This is a description of the glossary"
-    glossary = client.upsert(glossary).assets_created(AtlasGlossary)[0]
+    glossary = m_client.upsert(glossary).assets_created(AtlasGlossary)[0]
     glossary_term = AtlasGlossaryTerm.create(
         name="Integration Classification Term", anchor=glossary
     )
-    glossary_term = client.upsert(glossary_term).assets_created(AtlasGlossaryTerm)[0]
+    glossary_term = m_client.upsert(glossary_term).assets_created(AtlasGlossaryTerm)[0]
     qualified_name = glossary_term.attributes.qualified_name
     classification_name = "TEST"
-    client.add_classifications(AtlasGlossaryTerm, qualified_name, [classification_name])
-    glossary_term = client.get_asset_by_guid(
+    m_client.add_classifications(
+        AtlasGlossaryTerm, qualified_name, [classification_name]
+    )
+    glossary_term = m_client.get_asset_by_guid(
         glossary_term.guid, asset_type=AtlasGlossaryTerm
     )
     assert glossary_term.classifications
     assert len(glossary_term.classifications) == 1
     classification = glossary_term.classifications[0]
     assert str(classification.type_name) == classification_name
-    client.remove_classification(AtlasGlossaryTerm, qualified_name, classification_name)
-    glossary_term = client.get_asset_by_guid(
+    m_client.remove_classification(
+        AtlasGlossaryTerm, qualified_name, classification_name
+    )
+    glossary_term = m_client.get_asset_by_guid(
         glossary_term.guid, asset_type=AtlasGlossaryTerm
     )
     assert not glossary_term.classifications
 
 
-def test_create_for_modification(client: AtlanClient):
+def test_create_for_modification(m_client: AtlanClient):
     qualified_name = (
         "default/snowflake/1669038939/GREENE_HOMES_DEMO/STAGE/CONTRACT_STATUS"
     )
     classification_name = "TEST"
-    client.add_classifications(Table, qualified_name, [classification_name])
+    m_client.add_classifications(Table, qualified_name, [classification_name])
     table = Table.create_for_modification(
         qualified_name=qualified_name, name="CONTRACT_STATUS"
     )
-    response = client.upsert(table, replace_classifications=True)
+    response = m_client.upsert(table, replace_classifications=True)
     assert (tables := response.assets_updated(asset_type=Table))
     assert 1 == len(tables)
     assert tables[0].classifications is not None
     assert 0 == len(tables[0].classifications)
 
 
-def test_update_remove_certificate(client: AtlanClient):
+def test_update_remove_certificate(m_client: AtlanClient):
     glossary = AtlasGlossary.create(name="Integration Certificate Test")
     glossary.attributes.user_description = "This is a description of the glossary"
-    glossary = client.upsert(glossary).assets_created(AtlasGlossary)[0]
+    glossary = m_client.upsert(glossary).assets_created(AtlasGlossary)[0]
     message = "An important message"
-    asset = client.update_certificate(
+    asset = m_client.update_certificate(
         asset_type=AtlasGlossary,
         qualified_name=glossary.qualified_name,
         name=glossary.name,
         certificate_status=CertificateStatus.DRAFT,
         message=message,
     )
     assert asset is not None
     assert asset.certificate_status == CertificateStatus.DRAFT
     assert asset.certificate_status_message == message
-    asset = client.remove_certificate(
+    asset = m_client.remove_certificate(
         asset_type=AtlasGlossary,
         qualified_name=glossary.qualified_name,
         name=glossary.name,
     )
     assert asset is not None
     assert asset.certificate_status is None
     assert asset.certificate_status_message is None
 
 
-def test_update_remove_announcement(client: AtlanClient, announcement: Announcement):
+def test_update_remove_announcement(m_client: AtlanClient, announcement: Announcement):
     glossary = AtlasGlossary.create(name="Integration Announcement Test")
     glossary.attributes.user_description = "This is a description of the glossary"
-    glossary = client.upsert(glossary).assets_created(AtlasGlossary)[0]
-    asset = client.update_announcement(
+    glossary = m_client.upsert(glossary).assets_created(AtlasGlossary)[0]
+    asset = m_client.update_announcement(
         asset_type=AtlasGlossary,
         qualified_name=glossary.qualified_name,
         name=glossary.name,
         announcement=announcement,
     )
     assert asset is not None
     assert asset.get_announcment() == announcement
-    asset = client.remove_announcement(
+    asset = m_client.remove_announcement(
         asset_type=AtlasGlossary,
         qualified_name=glossary.qualified_name,
         name=glossary.name,
     )
     assert asset is not None
     assert asset.get_announcment() is None
 
 
-def test_create_readme(client: AtlanClient):
+def test_create_readme(m_client: AtlanClient):
     glossary = AtlasGlossary.create(name="Integration Readme Test")
     glossary.attributes.user_description = "This is a description of the glossary"
-    glossary = client.upsert(glossary).assets_created(AtlasGlossary)[0]
+    glossary = m_client.upsert(glossary).assets_created(AtlasGlossary)[0]
     readme = Readme.create(asset=glossary, content="<h1>Important</h1>")
-    response = client.upsert(readme)
+    response = m_client.upsert(readme)
     assert (reaadmes := response.assets_created(asset_type=Readme))
     assert len(reaadmes) == 1
     assert (glossaries := response.assets_updated(asset_type=AtlasGlossary))
     assert len(glossaries) == 1
 
 
 @pytest.fixture()
 def make_s3_object(
-    client: AtlanClient,
+    m_client: AtlanClient,
 ) -> Generator[Callable[[str], S3Object], None, None]:
     created_guids = []
-    connection = client.get_asset_by_guid(S3_CONNECTION_GUID, Connection)
+    connection = m_client.get_asset_by_guid(S3_CONNECTION_GUID, Connection)
 
     def _make_s3_object(name: str) -> S3Object:
         s3_object = S3Object.create(
             connection_qualified_name=connection.qualified_name,
             name=name,
             aws_arn=f"arn:aws:s3:::{name}",
         )
-        s3_object = client.upsert(s3_object).assets_created(S3Object)[0]
+        s3_object = m_client.upsert(s3_object).assets_created(S3Object)[0]
         created_guids.append(s3_object.guid)
         return s3_object
 
     yield _make_s3_object
 
     for guid in created_guids:
-        client.purge_entity_by_guid(guid=guid)
+        m_client.purge_entity_by_guid(guid=guid)
 
 
-def test_process_create(client: AtlanClient, make_s3_object: Callable[[str], S3Object]):
-    connection = client.get_asset_by_guid(S3_CONNECTION_GUID, Connection)
+def test_process_create(
+    m_client: AtlanClient, make_s3_object: Callable[[str], S3Object]
+):
+    connection = m_client.get_asset_by_guid(S3_CONNECTION_GUID, Connection)
 
     input_object = make_s3_object("Integration Source")
 
     output_object = make_s3_object("Integration Target")
 
     process = Process.create(
         name="Integration Process Test",
         connection_qualified_name=connection.qualified_name,
         process_id="doit",
         inputs=[input_object],
         outputs=[output_object],
     )
 
-    response = client.upsert(process)
+    response = m_client.upsert(process)
     assert (processes := response.assets_created(Process))
     assert len(processes) == 1
     assert (assets := response.assets_updated(S3Object))
     assert len(assets) == 2
```

### Comparing `pyatlan-0.0.31/tests/integration/test_index_search.py` & `pyatlan-0.0.32/tests/integration/test_index_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,16 +74,22 @@
 @dataclass()
 class AssetTracker:
     missing_types: set[str] = field(default_factory=set)
     found_types: set[str] = field(default_factory=set)
 
 
 @pytest.fixture(scope="module")
-def client() -> AtlanClient:
-    return AtlanClient()
+def m_client() -> AtlanClient:
+    from os import environ
+
+    client = AtlanClient(
+        base_url=environ["MARK_BASE_URL"], api_key=environ["MARK_API_KEY"]
+    )
+    AtlanClient.register_client(client)
+    return client
 
 
 @pytest.fixture(scope="module")
 def asset_tracker() -> Generator[AssetTracker, None, None]:
     tracker = AssetTracker()
     yield tracker
     print("Total number of asset types found: ", len(tracker.found_types))
@@ -103,84 +109,84 @@
         all_subclasses.append(subclass)
         all_subclasses.extend(get_all_subclasses(subclass))
 
     return all_subclasses
 
 
 @pytest.mark.parametrize("cls", [(cls) for cls in get_all_subclasses(Asset)])
-def test_search(client: AtlanClient, asset_tracker, cls):
+def test_search(m_client: AtlanClient, asset_tracker, cls):
     name = cls.__name__
     query = Term.with_state("ACTIVE")
     post_filter = Term.with_type_name(name)
     dsl = DSL(query=query, post_filter=post_filter)
     request = IndexSearchRequest(dsl=dsl, attributes=["name"])
-    results = client.search(criteria=request)
+    results = m_client.search(criteria=request)
     if results.count > 0:
         asset_tracker.found_types.add(name)
         counter = 0
         for asset in results:
             assert isinstance(asset, cls)
             counter += 1
             if counter > 3:
                 break
     else:
         asset_tracker.missing_types.add(name)
 
 
-def test_search_next_page(client: AtlanClient):
+def test_search_next_page(m_client: AtlanClient):
     size = 15
     dsl = DSL(
         query=Term.with_state("ACTIVE"),
         post_filter=Term.with_type_name(value="Database"),
         size=size,
     )
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["databaseName"],
     )
-    results = client.search(criteria=request)
+    results = m_client.search(criteria=request)
     assert results.count > size
     assert len(results.current_page()) == size
     counter = 0
     while True:
         for _ in results.current_page():
             counter += 1
         if results.next_page() is not True:
             break
     assert counter == results.count
 
 
-def test_search_iter(client: AtlanClient):
+def test_search_iter(m_client: AtlanClient):
     size = 15
     dsl = DSL(
         query=Term.with_state("ACTIVE"),
         post_filter=Term.with_type_name("Database"),
         size=size,
     )
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["databaseName"],
     )
-    results = client.search(criteria=request)
+    results = m_client.search(criteria=request)
     assert results.count > size
     assert len([a for a in results]) == results.count
 
 
-def test_search_next_when_start_changed_returns_remaining(client: AtlanClient):
+def test_search_next_when_start_changed_returns_remaining(m_client: AtlanClient):
     size = 2
     dsl = DSL(
         query=Term.with_state("ACTIVE"),
         post_filter=Term.with_type_name("Database"),
         size=size,
     )
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["databaseName"],
     )
-    results = client.search(criteria=request)
+    results = m_client.search(criteria=request)
     assert results.next_page(start=results.count - size) is True
     assert len(list(results)) == size
 
 
 @pytest.fixture()
 def term_query_value(request):
     return VALUES_FOR_TERM_QUERIES[request.param]
@@ -193,84 +199,89 @@
 
 @pytest.mark.parametrize(
     "term_query_value, method, clazz",
     [
         (method, method, query)
         for query in [Term, Prefix, Regexp, Wildcard]
         for method in sorted(dir(query))
-        if method.startswith("with_")
+        if method.startswith("with_") and method != "with_custom_metadata"
     ],
     indirect=["term_query_value"],
 )
-def test_term_queries_factory(client: AtlanClient, term_query_value, method, clazz):
+def test_term_queries_factory(m_client: AtlanClient, term_query_value, method, clazz):
     assert hasattr(clazz, method)
     query = getattr(clazz, method)(term_query_value)
     filter = ~Term.with_type_name("__AtlasAuditEntry")
     dsl = DSL(query=query, post_filter=filter, size=1)
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["name"],
     )
-    results = client.search(criteria=request)
+    results = m_client.search(criteria=request)
     assert results.count > 0
 
 
 @pytest.mark.parametrize(
-    "with_name", [(method) for method in dir(Exists) if method.startswith("with_")]
+    "with_name",
+    [
+        (method)
+        for method in dir(Exists)
+        if method.startswith("with_") and method != "with_custom_metadata"
+    ],
 )
-def test_exists_query_factory(client: AtlanClient, with_name):
+def test_exists_query_factory(m_client: AtlanClient, with_name):
     assert hasattr(Exists, with_name)
     query = getattr(Exists, with_name)()
     dsl = DSL(query=query, size=1)
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["name"],
     )
-    results = client.search(criteria=request)
+    results = m_client.search(criteria=request)
     assert results.count > 0
 
 
 @pytest.mark.parametrize(
     "text_query_value, method, clazz",
     [
         (method, method, query)
         for query in [Match]
         for method in sorted(dir(query))
         if method.startswith("with_")
     ],
     indirect=["text_query_value"],
 )
-def test_text_queries_factory(client: AtlanClient, text_query_value, method, clazz):
+def test_text_queries_factory(m_client: AtlanClient, text_query_value, method, clazz):
     assert hasattr(clazz, method)
     query = getattr(clazz, method)(text_query_value)
     filter = ~Term.with_type_name("__AtlasAuditEntry")
     dsl = DSL(query=query, post_filter=filter, size=1)
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["name"],
     )
     # print(request.json(by_alias=True, exclude_none=True))
-    results = client.search(criteria=request)
+    results = m_client.search(criteria=request)
     assert results.count > 0
 
 
 @pytest.mark.parametrize(
     "value, method, format",
     [
         (0, "with_popularity_score", None),
         (1665727666701, "with_create_time_as_timestamp", None),
         ("2023-01", "with_create_time_as_date", "yyyy-MM"),
         (1665727666701, "with_update_time_as_timestamp", None),
         ("2023-01", "with_update_time_as_date", "yyyy-MM"),
     ],
 )
-def test_range_factory(client: AtlanClient, value, method, format):
+def test_range_factory(m_client: AtlanClient, value, method, format):
     assert hasattr(Range, method)
     query = getattr(Range, method)(lt=value, format=format)
     filter = ~Term.with_type_name("__AtlasAuditEntry")
     dsl = DSL(query=query, post_filter=filter, size=1)
     request = IndexSearchRequest(
         dsl=dsl,
         attributes=["name"],
     )
-    results = client.search(criteria=request)
+    results = m_client.search(criteria=request)
     assert results.count > 0
```

### Comparing `pyatlan-0.0.31/tests/unit/test_classification_name.py` & `pyatlan-0.0.32/tests/unit/test_classification_name.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,12 +99,11 @@
 
     sut = ClassificationName._convert_to_display_text(CLASSIFICATION_ID)
 
     assert str(sut) == GOOD_CLASSIFICATION_NAME
 
 
 def test_json_encode_classification(monkeypatch, good_classification):
-
     assert (
         ClassificationName.json_encode_classification(good_classification)
         == CLASSIFICATION_ID
     )
```

### Comparing `pyatlan-0.0.31/tests/unit/test_client.py` & `pyatlan-0.0.32/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.31/tests/unit/test_glossary_term.py` & `pyatlan-0.0.32/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.31/tests/unit/test_lineage.py` & `pyatlan-0.0.32/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.0.31/tests/unit/test_model.py` & `pyatlan-0.0.32/tests/unit/test_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 
 import pytest
 from deepdiff import DeepDiff
 from pydantic.error_wrappers import ValidationError
 
 import pyatlan.cache.classification_cache
 from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
+from pyatlan.error import NotFoundError
 from pyatlan.model.assets import (
     ADLSAccountStatus,
     ADLSEncryptionTypes,
     ADLSReplicationType,
     Asset,
     AtlasGlossary,
     AtlasGlossaryCategory,
     AtlasGlossaryTerm,
     AtlasServer,
     AwsTag,
     AzureTag,
+    Badge,
     BadgeCondition,
     Catalog,
     ColumnValueFrequencyMap,
     Connection,
     Database,
     DbtMetricFilter,
     GoogleLabel,
@@ -51,42 +53,58 @@
     ADLSObjectArchiveStatus,
     ADLSObjectType,
     ADLSPerformance,
     ADLSProvisionState,
     ADLSStorageKind,
     AnnouncementType,
     AtlanConnectorType,
+    BadgeComparisonOperator,
+    BadgeConditionColor,
     CertificateStatus,
     GoogleDatastudioAssetType,
     IconType,
     KafkaTopicCompressionType,
     PowerbiEndorsement,
     QueryUsernameStrategy,
     QuickSightAnalysisStatus,
     QuickSightDatasetFieldType,
     QuickSightDatasetImportMode,
     QuickSightFolderType,
     SourceCostUnitType,
 )
 from pyatlan.model.response import AssetMutationResponse
-from pyatlan.model.structs import KafkaTopicConsumption
+from pyatlan.model.structs import (
+    KafkaTopicConsumption,
+    MCRuleComparison,
+    MCRuleSchedule,
+    SourceTagAttribute,
+)
 from pyatlan.model.typedef import TypeDefResponse
 
+CM_ATTR_ID = "WQ6XGXwq9o7UnZlkWyKhQN"
+
+CM_ID = "scAesIb5UhKQdTwu4GuCSN"
+
 SCHEMA_QUALIFIED_NAME = "default/snowflake/1646836521/ATLAN_SAMPLE_DATA/FOOD_BEVERAGE"
 
 TABLE_NAME = "MKT_EXPENSES"
 
 TABLE_URL = "POsWut55wIYsXZ5v4z3K98"
 
 FRESHNESS = "VdRC4dyNdTJHfFjCiNaKt9"
 
 MONTE_CARLO = "AFq4ctARP76ctapiTbuT92"
 
 MOON = "FAq4ctARP76ctapiTbuT92"
 
+BADGE_CONDITION = BadgeCondition.create(
+    badge_condition_operator=BadgeComparisonOperator.EQ,
+    badge_condition_value="1",
+    badge_condition_colorhex=BadgeConditionColor.RED,
+)
 DATA_DIR = Path(__file__).parent / "data"
 GLOSSARY_JSON = "glossary.json"
 GLOSSARY_TERM_JSON = "glossary_term.json"
 GLOSSARY_CATEGORY_JSON = "glossary_category.json"
 STRING_VALUE = "Bob"
 INT_VALUE = 42
 FLOAT_VALUE = 42.00
@@ -123,17 +141,20 @@
     "Optional[ADLSLeaseState]": ADLSLeaseState.LEASED,
     "Optional[ADLSLeaseStatus]": ADLSLeaseStatus.LOCKED,
     "Optional[ADLSObjectArchiveStatus]": ADLSObjectArchiveStatus.REHYDRATE_PENDING_TO_HOT,
     "Optional[ADLSObjectType]": ADLSObjectType.PAGE_BLOB,
     "Optional[PowerbiEndorsement]": PowerbiEndorsement.PROMOTED,
     "Optional[list[dict[str, str]]]": [{STRING_VALUE: STRING_VALUE}],
     "Optional[list[DbtMetricFilter]]": [DbtMetricFilter()],
+    "Optional[list[SourceTagAttribute]]": [SourceTagAttribute()],
     "Optional[Histogram]": Histogram(),
     "Optional[list[ColumnValueFrequencyMap]]": [ColumnValueFrequencyMap()],
     "Optional[KafkaTopicCompressionType]": KafkaTopicCompressionType.GZIP,
+    "Optional[MCRuleSchedule]": MCRuleSchedule(),
+    "Optional[list[MCRuleComparison]]": [MCRuleComparison()],
     "Optional[QuickSightFolderType]": QuickSightFolderType.SHARED,
     "Optional[QuickSightDatasetFieldType]": QuickSightDatasetFieldType.STRING,
     "Optional[QuickSightAnalysisStatus]": QuickSightAnalysisStatus.CREATION_FAILED,
     "Optional[QuickSightDatasetImportMode]": QuickSightDatasetImportMode.SPICE,
     "Optional[list[KafkaTopicConsumption]]": [KafkaTopicConsumption()],
     "list[AtlasGlossaryTerm]": [AtlasGlossaryTerm()],
 }
@@ -722,15 +743,14 @@
     [
         ("TestDB", "default/snowflake/1673868111909"),
     ],
 )
 def test_database_attributes_create_with_required_parameters(
     name, connection_qualified_name
 ):
-
     attributes = Database.Attributes.create(
         name=name, connection_qualified_name=connection_qualified_name
     )
     assert attributes.name == name
     assert attributes.connection_qualified_name == connection_qualified_name
     assert attributes.qualified_name == f"{connection_qualified_name}/{name}"
     assert attributes.connector_name == connection_qualified_name.split("/")[1]
@@ -758,15 +778,14 @@
 @pytest.mark.parametrize(
     "name, connection_qualified_name",
     [
         ("TestDB", "default/snowflake/1673868111909"),
     ],
 )
 def test_database_create_with_required_parameters(name, connection_qualified_name):
-
     database = Database.create(
         name=name, connection_qualified_name=connection_qualified_name
     )
     attributes = database.attributes
     assert attributes.name == name
     assert attributes.connection_qualified_name == connection_qualified_name
     assert attributes.qualified_name == f"{connection_qualified_name}/{name}"
@@ -1031,20 +1050,20 @@
     glossary = AtlasGlossary.create(name="Glossary")
     sut = AtlasGlossaryTerm.Attributes.create(name="Bob", anchor=glossary)
     assert sut.name == "Bob"
     assert sut.anchor == glossary
 
 
 @patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
-def test_get_business_attributes_when_name_not_valid_raises_value_error(
+def test_get_business_attributes_when_name_not_valid_raises_not_found_error(
     mock_client, table, type_def_response
 ):
     mock_client.return_value.get_typedefs.return_value = type_def_response
     with pytest.raises(
-        ValueError, match="No custom metadata with the name: Zoro exist"
+        NotFoundError, match="Custom metadata with name Zoro does not exist."
     ):
         table.get_custom_metadata("Zoro")
 
 
 @patch("pyatlan.cache.custom_metadata_cache.AtlanClient")
 def test_get_business_attributes_when_name_not_appropriate_for_asset_raises_value_error(
     mock_client, table, type_def_response
@@ -1099,15 +1118,14 @@
     ):
         table.set_custom_metadata({})
 
 
 def test_set_business_attributes_with_non_appropriate_meta_data_type_name_raises_value_error(
     table,
 ):
-
     with pytest.raises(
         ValueError,
         match="business_attributes must be an instance of CustomMetadata",
     ):
         table.set_custom_metadata({})
 
 
@@ -1383,15 +1401,14 @@
             "asset_name is required when name is not available from asset",
         ),
     ],
 )
 def test_create_readme_attributes_without_required_parameters_raises_exception(
     asset, content, asset_name, error, message
 ):
-
     with pytest.raises(error, match=message):
         Readme.Attributes.create(asset=asset, content=content, asset_name=asset_name)
 
 
 @pytest.mark.parametrize(
     "asset, content, asset_name, error, message",
     [
@@ -1421,15 +1438,14 @@
             "asset_name is required when name is not available from asset",
         ),
     ],
 )
 def test_create_readme_without_required_parameters_raises_exception(
     asset, content, asset_name, error, message
 ):
-
     with pytest.raises(error, match=message):
         Readme.create(asset=asset, content=content, asset_name=asset_name)
 
 
 @pytest.mark.parametrize(
     "asset, content, asset_name, expected_name",
     [
@@ -1656,7 +1672,182 @@
 
     assert process.name == name
     assert process.connection_qualified_name == connection_qualified_name
     assert process.qualified_name == expected_value
     assert process_id == process_id
     assert process.inputs == inputs
     assert process.outputs == outputs
+
+
+class Test_Badge_Attributes:
+    @pytest.mark.parametrize(
+        "name, cm_name, cm_attribute, badge_conditions, message",
+        [
+            (None, "Bob", "Dave", [BADGE_CONDITION], "name is required"),
+            ("Bob", None, "Dave", [BADGE_CONDITION], "cm_name is required"),
+            ("Bob", "", "Dave", [BADGE_CONDITION], "cm_name cannot be blank"),
+            ("Bob", "Dave", None, [BADGE_CONDITION], "cm_attribute is required"),
+            ("Bob", "Dave", "", [BADGE_CONDITION], "cm_attribute cannot be blank"),
+            ("Bob", "tom", "Dave", None, "badge_conditions is required"),
+            ("Bob", "tom", "Dave", [], "badge_conditions cannot be an empty list"),
+        ],
+    )
+    def test_create_when_required_parameters_are_missing_raises_value_error(
+        self, name, cm_name, cm_attribute, badge_conditions, message
+    ):
+        with pytest.raises(ValueError, match=message):
+            Badge.Attributes.create(
+                name=name,
+                cm_name=cm_name,
+                cm_attribute=cm_attribute,
+                badge_conditions=badge_conditions,
+            )
+
+    def test_create(self, monkeypatch):
+        def get_attr_id_for_name(set_name: str, attr_name: str):
+            return CM_ATTR_ID
+
+        def get_id_for_name(value):
+            return CM_ID
+
+        monkeypatch.setattr(
+            pyatlan.cache.custom_metadata_cache.CustomMetadataCache,
+            "get_id_for_name",
+            get_id_for_name,
+        )
+
+        monkeypatch.setattr(
+            pyatlan.cache.custom_metadata_cache.CustomMetadataCache,
+            "get_attr_id_for_name",
+            get_attr_id_for_name,
+        )
+
+        badge = Badge.Attributes.create(
+            name="bob",
+            cm_name="Monte Carlo",
+            cm_attribute="dummy",
+            badge_conditions=[BADGE_CONDITION],
+        )
+        assert badge.name == "bob"
+        assert badge.qualified_name == f"badges/global/{CM_ID}.{CM_ATTR_ID}"
+        assert badge.badge_metadata_attribute == f"{CM_ID}.{CM_ATTR_ID}"
+        assert badge.badge_conditions == [BADGE_CONDITION]
+
+
+class Test_Badge:
+    @pytest.mark.parametrize(
+        "name, cm_name, cm_attribute, badge_conditions, message",
+        [
+            (None, "Bob", "Dave", [BADGE_CONDITION], "name is required"),
+            ("Bob", None, "Dave", [BADGE_CONDITION], "cm_name is required"),
+            ("Bob", "", "Dave", [BADGE_CONDITION], "cm_name cannot be blank"),
+            ("Bob", "Dave", None, [BADGE_CONDITION], "cm_attribute is required"),
+            ("Bob", "Dave", "", [BADGE_CONDITION], "cm_attribute cannot be blank"),
+            ("Bob", "tom", "Dave", None, "badge_conditions is required"),
+            ("Bob", "tom", "Dave", [], "badge_conditions cannot be an empty list"),
+        ],
+    )
+    def test_create_when_required_parameters_are_missing_raises_value_error(
+        self, name, cm_name, cm_attribute, badge_conditions, message
+    ):
+        with pytest.raises(ValueError, match=message):
+            Badge.create(
+                name=name,
+                cm_name=cm_name,
+                cm_attribute=cm_attribute,
+                badge_conditions=badge_conditions,
+            )
+
+    def test_create(self, monkeypatch):
+        def get_attr_id_for_name(set_name: str, attr_name: str):
+            return CM_ATTR_ID
+
+        def get_id_for_name(value):
+            return CM_ID
+
+        monkeypatch.setattr(
+            pyatlan.cache.custom_metadata_cache.CustomMetadataCache,
+            "get_id_for_name",
+            get_id_for_name,
+        )
+
+        monkeypatch.setattr(
+            pyatlan.cache.custom_metadata_cache.CustomMetadataCache,
+            "get_attr_id_for_name",
+            get_attr_id_for_name,
+        )
+
+        badge = Badge.create(
+            name="bob",
+            cm_name="Monte Carlo",
+            cm_attribute="dummy",
+            badge_conditions=[BADGE_CONDITION],
+        )
+        assert badge.name == "bob"
+        assert badge.qualified_name == f"badges/global/{CM_ID}.{CM_ATTR_ID}"
+        assert badge.badge_metadata_attribute == f"{CM_ID}.{CM_ATTR_ID}"
+        assert badge.badge_conditions == [BADGE_CONDITION]
+
+
+class Test_BadgeCondition:
+    @pytest.mark.parametrize(
+        "condition_operator, condition_value, condition_colorhex, message",
+        [
+            (
+                None,
+                "1",
+                BadgeConditionColor.RED,
+                "badge_condition_operator is required",
+            ),
+            (
+                BadgeComparisonOperator.EQ,
+                None,
+                BadgeConditionColor.RED,
+                "badge_condition_value is required",
+            ),
+            (
+                BadgeComparisonOperator.EQ,
+                "1",
+                None,
+                "badge_condition_colorhex is required",
+            ),
+        ],
+    )
+    def test_create_when_required_parameter_is_missing_then_raises_value_error(
+        self, condition_operator, condition_value, condition_colorhex, message
+    ):
+        with pytest.raises(ValueError, match=message):
+            BadgeCondition.create(
+                badge_condition_operator=condition_operator,
+                badge_condition_value=condition_value,
+                badge_condition_colorhex=condition_colorhex,
+            )
+
+    def test_create_with_badge_condition_color(self):
+        condition_operator = BadgeComparisonOperator.EQ
+        condition_value = "1"
+        condition_colorhex = BadgeConditionColor.RED
+
+        sut = BadgeCondition.create(
+            badge_condition_operator=condition_operator,
+            badge_condition_value=condition_value,
+            badge_condition_colorhex=condition_colorhex,
+        )
+
+        assert sut.badge_condition_operator == condition_operator.value
+        assert sut.badge_condition_value == condition_value
+        assert sut.badge_condition_colorhex == condition_colorhex.value
+
+    def test_create_with_badge_condition_color_as_str(self):
+        condition_operator = BadgeComparisonOperator.EQ
+        condition_value = "1"
+        condition_colorhex = "#BF1B1B"
+
+        sut = BadgeCondition.create(
+            badge_condition_operator=condition_operator,
+            badge_condition_value=condition_value,
+            badge_condition_colorhex=condition_colorhex,
+        )
+
+        assert sut.badge_condition_operator == condition_operator.value
+        assert sut.badge_condition_value == condition_value
+        assert sut.badge_condition_colorhex == condition_colorhex
```

### Comparing `pyatlan-0.0.31/tests/unit/test_search_model.py` & `pyatlan-0.0.32/tests/unit/test_search_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,14 @@
             },
         ),
     ],
 )
 def test_bool_to_dict_without_optional_fields(
     must, should, must_not, filter, boost, minimum_should_match, expected
 ):
-
     assert (
         Bool(
             must=must,
             should=should,
             must_not=must_not,
             filter=filter,
             boost=boost,
```

### Comparing `pyatlan-0.0.31/tests/unit/test_typedef_model.py` & `pyatlan-0.0.32/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

