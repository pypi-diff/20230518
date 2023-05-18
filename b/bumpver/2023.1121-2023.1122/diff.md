# Comparing `tmp/bumpver-2023.1121.tar.gz` & `tmp/bumpver-2023.1122.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumpver-2023.1121.tar", last modified: Thu May  4 16:35:11 2023, max compression
+gzip compressed data, was "bumpver-2023.1122.tar", last modified: Thu May 18 14:55:45 2023, max compression
```

## Comparing `bumpver-2023.1121.tar` & `bumpver-2023.1122.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.679573 bumpver-2023.1121/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     8986 2023-05-04 16:01:47.000000 bumpver-2023.1121/CHANGELOG.md
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1127 2023-05-04 16:02:43.000000 bumpver-2023.1121/LICENSE
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      148 2023-05-04 13:50:20.000000 bumpver-2023.1121/MANIFEST.in
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    50255 2023-05-04 16:35:11.679573 bumpver-2023.1121/PKG-INFO
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    40087 2023-05-04 16:02:43.000000 bumpver-2023.1121/README.md
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     4053 2023-05-04 13:50:20.000000 bumpver-2023.1121/fastentrypoints.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:09.968430 bumpver-2023.1121/requirements/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      697 2023-05-04 14:52:41.000000 bumpver-2023.1121/requirements/pypi.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2370 2023-05-04 16:35:11.679573 bumpver-2023.1121/setup.cfg
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2457 2023-05-04 16:02:43.000000 bumpver-2023.1121/setup.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:09.735361 bumpver-2023.1121/src/
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:10.657263 bumpver-2023.1121/src/bumpver/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      262 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/__init__.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      363 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/__main__.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    25569 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/cli.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    21008 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/config.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2548 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/parse.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      793 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/patterns.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1214 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/pysix.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2267 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/regexfmt.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2290 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/rewrite.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      612 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/utils.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     7915 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v1patterns.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     5257 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v1rewrite.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    13411 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v1version.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    11045 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v2patterns.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     5736 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v2rewrite.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    28055 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/v2version.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     8275 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/vcs.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     4177 2023-05-04 16:02:43.000000 bumpver-2023.1121/src/bumpver/version.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.054247 bumpver-2023.1121/src/bumpver.egg-info/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    50255 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/PKG-INFO
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1262 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/SOURCES.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/dependency_links.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       44 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/entry_points.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      198 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/requires.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        8 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/top_level.txt
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2023-05-04 16:35:09.000000 bumpver-2023.1121/src/bumpver.egg-info/zip-safe
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.271266 bumpver-2023.1121/test/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/__init__.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:09.817424 bumpver-2023.1121/test/fixtures/
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.335332 bumpver-2023.1121/test/fixtures/project_a/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       66 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_a/README.md
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      266 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_a/bumpver.toml
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.460004 bumpver-2023.1121/test/fixtures/project_b/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      219 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_b/README.rst
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      461 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_b/setup.cfg
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      136 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_b/setup.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:09.797842 bumpver-2023.1121/test/fixtures/project_b/src/
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.506882 bumpver-2023.1121/test/fixtures/project_b/src/module_v1/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       34 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_b/src/module_v1/__init__.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.569787 bumpver-2023.1121/test/fixtures/project_b/src/module_v2/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       34 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_b/src/module_v2/__init__.py
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.601036 bumpver-2023.1121/test/fixtures/project_c/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      135 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/fixtures/project_c/pyproject.toml
-drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 16:35:11.648322 bumpver-2023.1121/test/fixtures/project_d/
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      114 2023-05-04 16:02:18.000000 bumpver-2023.1121/test/fixtures/project_d/pyproject.toml
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    42098 2023-05-04 16:01:47.000000 bumpver-2023.1121/test/test_cli.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    11574 2023-05-04 16:02:18.000000 bumpver-2023.1121/test/test_config.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2381 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/test_parse.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     9708 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/test_patterns.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    12813 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/test_rewrite.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    10453 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/test_version.py
--rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2481 2023-05-04 13:50:20.000000 bumpver-2023.1121/test/util.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:45.932204 bumpver-2023.1122/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     9217 2023-05-18 14:55:21.000000 bumpver-2023.1122/CHANGELOG.md
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1127 2023-05-18 14:55:34.000000 bumpver-2023.1122/LICENSE
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      148 2023-05-04 13:50:20.000000 bumpver-2023.1122/MANIFEST.in
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    50680 2023-05-18 14:55:45.934826 bumpver-2023.1122/PKG-INFO
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    40281 2023-05-18 14:55:34.000000 bumpver-2023.1122/README.md
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     4053 2023-05-04 13:50:20.000000 bumpver-2023.1122/fastentrypoints.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:44.281266 bumpver-2023.1122/requirements/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      697 2023-05-04 14:52:41.000000 bumpver-2023.1122/requirements/pypi.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2370 2023-05-18 14:55:45.947237 bumpver-2023.1122/setup.cfg
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2457 2023-05-18 14:55:34.000000 bumpver-2023.1122/setup.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:44.077947 bumpver-2023.1122/src/
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:44.965507 bumpver-2023.1122/src/bumpver/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      262 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/__init__.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      363 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/__main__.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    25865 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/cli.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    21008 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/config.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2548 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/parse.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      793 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1214 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/pysix.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2267 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/regexfmt.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2290 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      612 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/utils.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     7915 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/v1patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     5257 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/v1rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    13411 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/v1version.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    11045 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/v2patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     5736 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/v2rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    28055 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/v2version.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     8275 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/vcs.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     4177 2023-05-18 14:55:34.000000 bumpver-2023.1122/src/bumpver/version.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:45.191396 bumpver-2023.1122/src/bumpver.egg-info/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    50680 2023-05-18 14:55:43.000000 bumpver-2023.1122/src/bumpver.egg-info/PKG-INFO
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1262 2023-05-18 14:55:44.000000 bumpver-2023.1122/src/bumpver.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2023-05-18 14:55:43.000000 bumpver-2023.1122/src/bumpver.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       44 2023-05-18 14:55:43.000000 bumpver-2023.1122/src/bumpver.egg-info/entry_points.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      198 2023-05-18 14:55:43.000000 bumpver-2023.1122/src/bumpver.egg-info/requires.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        8 2023-05-18 14:55:43.000000 bumpver-2023.1122/src/bumpver.egg-info/top_level.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2023-05-18 14:55:43.000000 bumpver-2023.1122/src/bumpver.egg-info/zip-safe
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:45.412278 bumpver-2023.1122/test/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/__init__.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:44.146761 bumpver-2023.1122/test/fixtures/
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:45.498462 bumpver-2023.1122/test/fixtures/project_a/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       66 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/fixtures/project_a/README.md
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      266 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/fixtures/project_a/bumpver.toml
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:45.629725 bumpver-2023.1122/test/fixtures/project_b/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      219 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/fixtures/project_b/README.rst
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      461 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/fixtures/project_b/setup.cfg
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      136 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/fixtures/project_b/setup.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:44.129877 bumpver-2023.1122/test/fixtures/project_b/src/
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:45.688107 bumpver-2023.1122/test/fixtures/project_b/src/module_v1/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       34 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/fixtures/project_b/src/module_v1/__init__.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:45.751535 bumpver-2023.1122/test/fixtures/project_b/src/module_v2/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       34 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/fixtures/project_b/src/module_v2/__init__.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:45.801021 bumpver-2023.1122/test/fixtures/project_c/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      135 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/fixtures/project_c/pyproject.toml
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2023-05-18 14:55:45.866772 bumpver-2023.1122/test/fixtures/project_d/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      114 2023-05-04 16:02:18.000000 bumpver-2023.1122/test/fixtures/project_d/pyproject.toml
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    43298 2023-05-18 14:55:21.000000 bumpver-2023.1122/test/test_cli.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    11574 2023-05-04 16:02:18.000000 bumpver-2023.1122/test/test_config.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2381 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/test_parse.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     9708 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/test_patterns.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    12813 2023-05-04 16:45:20.000000 bumpver-2023.1122/test/test_rewrite.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    10996 2023-05-18 14:55:21.000000 bumpver-2023.1122/test/test_version.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2481 2023-05-04 13:50:20.000000 bumpver-2023.1122/test/util.py
```

### Comparing `bumpver-2023.1121/CHANGELOG.md` & `bumpver-2023.1122/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog for https://github.com/mbarkhau/bumpver
 
+## BumpVer 2023.1122
+
+- Fix [#207][gh_i207]: Add --ignore-vcs-tag for old version support purpose
+
+[gh_i207]: https://github.com/mbarkhau/bumpver/issues/207
+
+Thank you [Jusong Yu](https://github.com/unkcpz) for your contribution.
+
 ## BumpVer 2023.1121
 
 - Fix [#200][gh_i200]: Fix compatability with packaging 23.0.
 - Fix [#203][gh_i203]: Add dev to the list of valid release tags
 
 [gh_i200]: https://github.com/mbarkhau/bumpver/issues/200
 [gh_i203]: https://github.com/mbarkhau/bumpver/issues/203
```

### Comparing `bumpver-2023.1121/LICENSE` & `bumpver-2023.1122/LICENSE`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/PKG-INFO` & `bumpver-2023.1122/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpver
-Version: 2023.1121
+Version: 2023.1122
 Summary: Bump version numbers in project files.
 Home-page: https://github.com/mbarkhau/bumpver
 Author: Manuel Barkhau
 Author-email: mbarkhau@gmail.com
 License: MIT
 Keywords: version bumpver calver semver versioning bumpversion pep440
 Classifier: Development Status :: 4 - Beta
@@ -47,15 +47,15 @@
 [url_calver_org]: https://calver.org/
 
 
 Project/Repo:
 
 [![MIT License][img_license]][url_license]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
-[![CalVer 2023.1121][img_version]][url_version]
+[![CalVer 2023.1122][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![PyPI Downloads][img_downloads]][url_downloads]
 
 Code Quality/CI:
 
 [![GitHub Build Status][img_github_build]][url_github_build]
 [![GitLab Build Status][img_gitlab_build]][url_gitlab_build]
@@ -81,15 +81,15 @@
 
 [img_style]: https://img.shields.io/badge/code%20style-%20sjfmt-f71.svg
 [url_style]: https://gitlab.com/mbarkhau/straitjacket/
 
 [img_downloads]: https://pepy.tech/badge/bumpver/month
 [url_downloads]: https://pepy.tech/project/bumpver
 
-[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1121&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1122&color=blue
 [url_version]: https://pypi.org/project/bumpver/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/bumpver/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/bumpver.svg
 [url_pyversions]: https://pypi.python.org/pypi/bumpver
@@ -597,16 +597,16 @@
 $ bumpver --help
 Usage: bumpver [OPTIONS] COMMAND [ARGS]...
 
   Automatically update version strings in plaintext files.
 
 Options:
   --version      Show the version and exit.
-  --help         Show this message and exit.
   -v, --verbose  Control log level. -vv for debug level.
+  -h, --help     Show this message and exit.
 
 Commands:
   grep    Search file(s) for a version pattern.
   init    Initialize [bumpver] configuration.
   show    Show current version of your project.
   test    Increment a version number for demo purposes.
   update  Update project files with the incremented version string.
@@ -619,38 +619,43 @@
 ```
 $ bumpver update --help
 Usage: bumpver update [OPTIONS]
 
   Update project files with the incremented version string.
 
 Options:
-  -d, --dry                       Display diff of changes, don't rewrite files.
+  -d, --dry                       Display diff of changes, don't rewrite
+                                  files.
   -f, --fetch / -n, --no-fetch    Sync tags from remote origin.
   -v, --verbose                   Control log level. -vv for debug level.
   --allow-dirty                   Commit even when working directory is has
-                                  uncomitted changes. (WARNING: The commit will
-                                  still be aborted if there are uncomitted to
-                                  files with version strings.
+                                  uncomitted changes. (WARNING: The commit
+                                  will still be aborted if there are
+                                  uncomitted to files with version strings.
+  --ignore-vcs-tag                Ignore VCS tag invariant and update version
+                                  anyway.
   --set-version <VERSION>         Set version explicitly.
   --date <ISODATE>                Set explicit date in format YYYY-0M-0D (e.g.
-                                  2021-05-13).
+                                  2023-05-18).
   --pin-date                      Leave date components unchanged.
   --pin-increments                Leave the auto-increments INC0 and INC1
+                                  unchanged.
   --tag-num                       Increment release tag number (rc1, rc2,
                                   rc3..).
-  -t, --tag <NAME>                Override release tag of current_version. Valid
-                                  options are: alpha, beta, dev, rc, post, final.
+  -t, --tag <NAME>                Override release tag of current_version.
+                                  Valid options are: alpha, beta, dev, rc,
+                                  post, final.
   -p, --patch                     Increment PATCH component.
   -m, --minor                     Increment MINOR component.
   --major                         Increment MAJOR component.
   -c, --commit-message <TMPL>     Set commit message template.
   --commit / --no-commit          Create a commit with all updated files.
   --tag-commit / --no-tag-commit  Tag the newly created commit.
   --push / --no-push              Push to the default remote.
-  --help                          Show this message and exit.
+  -h, --help                      Show this message and exit.
 ```
 
 <!-- END bumpver update --help -->
 
 To help with shell script automation, you can use `bumpver show --env`.
 
 ```shell
@@ -754,32 +759,32 @@
 [pep_440_normalzation_ref]: https://www.python.org/dev/peps/pep-0440/#id31
 
 
 ### Pattern Examples
 
 <!-- BEGIN pattern_examples -->
 
-|             pattern             |               examples              | PEP440 | lexico. |
-|---------------------------------|-------------------------------------|--------|---------|
-| `MAJOR.MINOR.PATCH[PYTAGNUM]`   | `0.13.10          0.16.10rc1`       | yes    | no      |
-| `MAJOR.MINOR[.PATCH[PYTAGNUM]]` | `1.11             0.3.0b5`          | yes    | no      |
-| `YYYY.BUILD[PYTAGNUM]`          | `2020.1031        2020.1148a0`      | yes    | yes     |
-| `YYYY.BUILD[-TAG]`              | `2021.1393-beta   2022.1279`        | no     | yes     |
-| `YYYY.INC0[PYTAGNUM]`           | `2020.10          2021.12b2`        | yes    | no      |
-| `YYYY0M.PATCH[-TAG]`            | `202005.12        202210.15-beta`   | no     | no¹     |
-| `YYYY0M.BUILD[-TAG]`            | `202106.1071      202106.1075-beta` | no     | yes     |
-| `YYYY.0M`                       | `2020.02          2022.09`          | no     | yes     |
-| `YYYY.MM`                       | `2020.8           2020.10`          | yes    | no      |
-| `YYYY.WW`                       | `2020.8           2021.14`          | yes    | no      |
-| `YYYY.MM.PATCH[PYTAGNUM]`       | `2020.3.12b0      2021.6.19b0`      | yes    | no      |
-| `YYYY.0M.PATCH[PYTAGNUM]`       | `2020.10.15b0     2022.07.7b0`      | no     | no¹     |
-| `YYYY.MM.INC0`                  | `2021.6.2         2022.8.9`         | yes    | no      |
-| `YYYY.MM.DD`                    | `2020.5.18        2021.8.2`         | yes    | no      |
-| `YYYY.0M.0D`                    | `2020.08.24       2022.05.03`       | no     | yes     |
-| `YY.0M.PATCH`                   | `21.04.2          21.11.12`         | no     | no²     |
+| pattern                         | examples                          | PEP440 | lexico. |
+|---------------------------------|-----------------------------------|--------|---------|
+| `MAJOR.MINOR.PATCH[PYTAGNUM]`   | `0.13.10          0.16.10`        | yes    | no      |
+| `MAJOR.MINOR[.PATCH[PYTAGNUM]]` | `0.11.15          0.16.18`        | yes    | no      |
+| `YYYY.BUILD[PYTAGNUM]`          | `2020.1031        2020.1406`      | yes    | yes     |
+| `YYYY.BUILD[-TAG]`              | `2021.1393-beta   2022.1279`      | no     | yes     |
+| `YYYY.INC0[PYTAGNUM]`           | `2020.4b0         2020.16`        | yes    | no      |
+| `YYYY0M.PATCH[-TAG]`            | `202210.10        202211.13-beta` | no     | no¹     |
+| `YYYY0M.BUILD[-TAG]`            | `202005.1269-beta 202206.1056`    | no     | yes     |
+| `YYYY.0M`                       | `2020.01          2021.04`        | no     | yes     |
+| `YYYY.MM`                       | `2020.2           2022.2`         | yes    | no      |
+| `YYYY.WW`                       | `2020.33          2020.39`        | yes    | no      |
+| `YYYY.MM.PATCH[PYTAGNUM]`       | `2022.3.1b0       2022.11.15b0`   | yes    | no      |
+| `YYYY.0M.PATCH[PYTAGNUM]`       | `2020.03.2        2022.02.4`      | no     | no¹     |
+| `YYYY.MM.INC0`                  | `2020.7.10        2021.7.7`       | yes    | no      |
+| `YYYY.MM.DD`                    | `2020.8.9         2020.8.20`      | yes    | no      |
+| `YYYY.0M.0D`                    | `2020.11.02       2022.05.03`     | no     | yes     |
+| `YY.0M.PATCH`                   | `20.05.12         22.03.5`        | no     | no²     |
 
 <!-- END pattern_examples -->
 
 - ¹ If `PATCH > 9`
 - ² For the year 2100, the part `YY` will produce 0
 
 
@@ -794,15 +799,15 @@
 If you use `VV`/`0V`, be aware that you cannot also use `YYYY`.
 Instead use `GGGG`. This is to avoid an edge case where your version
 number would run backwards if it was created around New Year.
 
 
 <!-- BEGIN weeknum_example -->
 
-```sql
+```
                    YYYY WW UU  GGGG VV
 2020-12-26 (Sat):  2020 51 51  2020 52
 2020-12-27 (Sun):  2020 51 52  2020 52
 2020-12-28 (Mon):  2020 52 52  2020 53
 2020-12-29 (Tue):  2020 52 52  2020 53
 2020-12-30 (Wed):  2020 52 52  2020 53
 2020-12-31 (Thu):  2020 52 52  2020 53
@@ -821,15 +826,15 @@
 
 The create an initial configuration for project with `bumpver init`.
 
 ```shell
 $ pip install bumpver
 ...
 Installing collected packages: click toml lexid bumpver
-Successfully installed bumpver-2023.1121
+Successfully installed bumpver-2023.1122
 
 $ cd myproject
 ~/myproject/
 
 $ bumpver init --dry
 Exiting because of '-d/--dry'. Would have written to bumpver.toml:
 
@@ -1117,14 +1122,22 @@
 |                Name                 |    role           |  since  | until |
 |-------------------------------------|-------------------|---------|-------|
 | Manuel Barkhau (mbarkhau@gmail.com) | author/maintainer | 2018-09 | -     |
 
 
 # Changelog for https://github.com/mbarkhau/bumpver
 
+## BumpVer 2023.1122
+
+- Fix [#207][gh_i207]: Add --ignore-vcs-tag for old version support purpose
+
+[gh_i207]: https://github.com/mbarkhau/bumpver/issues/207
+
+Thank you [Jusong Yu](https://github.com/unkcpz) for your contribution.
+
 ## BumpVer 2023.1121
 
 - Fix [#200][gh_i200]: Fix compatability with packaging 23.0.
 - Fix [#203][gh_i203]: Add dev to the list of valid release tags
 
 [gh_i200]: https://github.com/mbarkhau/bumpver/issues/200
 [gh_i203]: https://github.com/mbarkhau/bumpver/issues/203
```

### Comparing `bumpver-2023.1121/README.md` & `bumpver-2023.1122/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [url_calver_org]: https://calver.org/
 
 
 Project/Repo:
 
 [![MIT License][img_license]][url_license]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
-[![CalVer 2023.1121][img_version]][url_version]
+[![CalVer 2023.1122][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![PyPI Downloads][img_downloads]][url_downloads]
 
 Code Quality/CI:
 
 [![GitHub Build Status][img_github_build]][url_github_build]
 [![GitLab Build Status][img_gitlab_build]][url_gitlab_build]
@@ -52,15 +52,15 @@
 
 [img_style]: https://img.shields.io/badge/code%20style-%20sjfmt-f71.svg
 [url_style]: https://gitlab.com/mbarkhau/straitjacket/
 
 [img_downloads]: https://pepy.tech/badge/bumpver/month
 [url_downloads]: https://pepy.tech/project/bumpver
 
-[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1121&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1122&color=blue
 [url_version]: https://pypi.org/project/bumpver/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/bumpver/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/bumpver.svg
 [url_pyversions]: https://pypi.python.org/pypi/bumpver
@@ -568,16 +568,16 @@
 $ bumpver --help
 Usage: bumpver [OPTIONS] COMMAND [ARGS]...
 
   Automatically update version strings in plaintext files.
 
 Options:
   --version      Show the version and exit.
-  --help         Show this message and exit.
   -v, --verbose  Control log level. -vv for debug level.
+  -h, --help     Show this message and exit.
 
 Commands:
   grep    Search file(s) for a version pattern.
   init    Initialize [bumpver] configuration.
   show    Show current version of your project.
   test    Increment a version number for demo purposes.
   update  Update project files with the incremented version string.
@@ -590,38 +590,43 @@
 ```
 $ bumpver update --help
 Usage: bumpver update [OPTIONS]
 
   Update project files with the incremented version string.
 
 Options:
-  -d, --dry                       Display diff of changes, don't rewrite files.
+  -d, --dry                       Display diff of changes, don't rewrite
+                                  files.
   -f, --fetch / -n, --no-fetch    Sync tags from remote origin.
   -v, --verbose                   Control log level. -vv for debug level.
   --allow-dirty                   Commit even when working directory is has
-                                  uncomitted changes. (WARNING: The commit will
-                                  still be aborted if there are uncomitted to
-                                  files with version strings.
+                                  uncomitted changes. (WARNING: The commit
+                                  will still be aborted if there are
+                                  uncomitted to files with version strings.
+  --ignore-vcs-tag                Ignore VCS tag invariant and update version
+                                  anyway.
   --set-version <VERSION>         Set version explicitly.
   --date <ISODATE>                Set explicit date in format YYYY-0M-0D (e.g.
-                                  2021-05-13).
+                                  2023-05-18).
   --pin-date                      Leave date components unchanged.
   --pin-increments                Leave the auto-increments INC0 and INC1
+                                  unchanged.
   --tag-num                       Increment release tag number (rc1, rc2,
                                   rc3..).
-  -t, --tag <NAME>                Override release tag of current_version. Valid
-                                  options are: alpha, beta, dev, rc, post, final.
+  -t, --tag <NAME>                Override release tag of current_version.
+                                  Valid options are: alpha, beta, dev, rc,
+                                  post, final.
   -p, --patch                     Increment PATCH component.
   -m, --minor                     Increment MINOR component.
   --major                         Increment MAJOR component.
   -c, --commit-message <TMPL>     Set commit message template.
   --commit / --no-commit          Create a commit with all updated files.
   --tag-commit / --no-tag-commit  Tag the newly created commit.
   --push / --no-push              Push to the default remote.
-  --help                          Show this message and exit.
+  -h, --help                      Show this message and exit.
 ```
 
 <!-- END bumpver update --help -->
 
 To help with shell script automation, you can use `bumpver show --env`.
 
 ```shell
@@ -725,32 +730,32 @@
 [pep_440_normalzation_ref]: https://www.python.org/dev/peps/pep-0440/#id31
 
 
 ### Pattern Examples
 
 <!-- BEGIN pattern_examples -->
 
-|             pattern             |               examples              | PEP440 | lexico. |
-|---------------------------------|-------------------------------------|--------|---------|
-| `MAJOR.MINOR.PATCH[PYTAGNUM]`   | `0.13.10          0.16.10rc1`       | yes    | no      |
-| `MAJOR.MINOR[.PATCH[PYTAGNUM]]` | `1.11             0.3.0b5`          | yes    | no      |
-| `YYYY.BUILD[PYTAGNUM]`          | `2020.1031        2020.1148a0`      | yes    | yes     |
-| `YYYY.BUILD[-TAG]`              | `2021.1393-beta   2022.1279`        | no     | yes     |
-| `YYYY.INC0[PYTAGNUM]`           | `2020.10          2021.12b2`        | yes    | no      |
-| `YYYY0M.PATCH[-TAG]`            | `202005.12        202210.15-beta`   | no     | no¹     |
-| `YYYY0M.BUILD[-TAG]`            | `202106.1071      202106.1075-beta` | no     | yes     |
-| `YYYY.0M`                       | `2020.02          2022.09`          | no     | yes     |
-| `YYYY.MM`                       | `2020.8           2020.10`          | yes    | no      |
-| `YYYY.WW`                       | `2020.8           2021.14`          | yes    | no      |
-| `YYYY.MM.PATCH[PYTAGNUM]`       | `2020.3.12b0      2021.6.19b0`      | yes    | no      |
-| `YYYY.0M.PATCH[PYTAGNUM]`       | `2020.10.15b0     2022.07.7b0`      | no     | no¹     |
-| `YYYY.MM.INC0`                  | `2021.6.2         2022.8.9`         | yes    | no      |
-| `YYYY.MM.DD`                    | `2020.5.18        2021.8.2`         | yes    | no      |
-| `YYYY.0M.0D`                    | `2020.08.24       2022.05.03`       | no     | yes     |
-| `YY.0M.PATCH`                   | `21.04.2          21.11.12`         | no     | no²     |
+| pattern                         | examples                          | PEP440 | lexico. |
+|---------------------------------|-----------------------------------|--------|---------|
+| `MAJOR.MINOR.PATCH[PYTAGNUM]`   | `0.13.10          0.16.10`        | yes    | no      |
+| `MAJOR.MINOR[.PATCH[PYTAGNUM]]` | `0.11.15          0.16.18`        | yes    | no      |
+| `YYYY.BUILD[PYTAGNUM]`          | `2020.1031        2020.1406`      | yes    | yes     |
+| `YYYY.BUILD[-TAG]`              | `2021.1393-beta   2022.1279`      | no     | yes     |
+| `YYYY.INC0[PYTAGNUM]`           | `2020.4b0         2020.16`        | yes    | no      |
+| `YYYY0M.PATCH[-TAG]`            | `202210.10        202211.13-beta` | no     | no¹     |
+| `YYYY0M.BUILD[-TAG]`            | `202005.1269-beta 202206.1056`    | no     | yes     |
+| `YYYY.0M`                       | `2020.01          2021.04`        | no     | yes     |
+| `YYYY.MM`                       | `2020.2           2022.2`         | yes    | no      |
+| `YYYY.WW`                       | `2020.33          2020.39`        | yes    | no      |
+| `YYYY.MM.PATCH[PYTAGNUM]`       | `2022.3.1b0       2022.11.15b0`   | yes    | no      |
+| `YYYY.0M.PATCH[PYTAGNUM]`       | `2020.03.2        2022.02.4`      | no     | no¹     |
+| `YYYY.MM.INC0`                  | `2020.7.10        2021.7.7`       | yes    | no      |
+| `YYYY.MM.DD`                    | `2020.8.9         2020.8.20`      | yes    | no      |
+| `YYYY.0M.0D`                    | `2020.11.02       2022.05.03`     | no     | yes     |
+| `YY.0M.PATCH`                   | `20.05.12         22.03.5`        | no     | no²     |
 
 <!-- END pattern_examples -->
 
 - ¹ If `PATCH > 9`
 - ² For the year 2100, the part `YY` will produce 0
 
 
@@ -765,15 +770,15 @@
 If you use `VV`/`0V`, be aware that you cannot also use `YYYY`.
 Instead use `GGGG`. This is to avoid an edge case where your version
 number would run backwards if it was created around New Year.
 
 
 <!-- BEGIN weeknum_example -->
 
-```sql
+```
                    YYYY WW UU  GGGG VV
 2020-12-26 (Sat):  2020 51 51  2020 52
 2020-12-27 (Sun):  2020 51 52  2020 52
 2020-12-28 (Mon):  2020 52 52  2020 53
 2020-12-29 (Tue):  2020 52 52  2020 53
 2020-12-30 (Wed):  2020 52 52  2020 53
 2020-12-31 (Thu):  2020 52 52  2020 53
@@ -792,15 +797,15 @@
 
 The create an initial configuration for project with `bumpver init`.
 
 ```shell
 $ pip install bumpver
 ...
 Installing collected packages: click toml lexid bumpver
-Successfully installed bumpver-2023.1121
+Successfully installed bumpver-2023.1122
 
 $ cd myproject
 ~/myproject/
 
 $ bumpver init --dry
 Exiting because of '-d/--dry'. Would have written to bumpver.toml:
```

### Comparing `bumpver-2023.1121/fastentrypoints.py` & `bumpver-2023.1122/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/requirements/pypi.txt` & `bumpver-2023.1122/requirements/pypi.txt`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/setup.cfg` & `bumpver-2023.1122/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 	dist/
 	.mypy_cache
 
 [tool:pytest]
 addopts = --doctest-modules
 
 [bumpver]
-current_version = "2023.1121"
+current_version = "2023.1122"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

### Comparing `bumpver-2023.1121/setup.py` & `bumpver-2023.1122/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 setuptools.setup(
     name="bumpver",
     license="MIT",
     author="Manuel Barkhau",
     author_email="mbarkhau@gmail.com",
     url="https://github.com/mbarkhau/bumpver",
-    version="2023.1121",
+    version="2023.1122",
     keywords="version bumpver calver semver versioning bumpversion pep440",
     description="Bump version numbers in project files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages("src"),
     package_dir=package_dir,
     install_requires=install_requires,
```

### Comparing `bumpver-2023.1121/src/bumpver/cli.py` & `bumpver-2023.1122/src/bumpver/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,15 @@
     decorated = function
     for decorator in decorators:
         decorated = decorator(decorated)
     return decorated
 
 
 @click.group(context_settings={'help_option_names': ["-h", "--help"]})
-@click.version_option(version="2023.1121")
+@click.version_option(version="2023.1122")
 @verbose_option
 def cli(verbose: int = 0) -> None:
     """Automatically update version strings in plaintext files."""
     if verbose:
         _configure_logging(verbose=max(_VERBOSE, verbose))
 
 
@@ -516,14 +516,15 @@
     except version.PatternError:
         logger.error(f"Invalid version '{new_version}' for pattern '{raw_pattern}'")
         return False
 
     if version.parse_version(new_version) <= version.parse_version(old_version):
         logger.error("Invariant violated: New version must be greater than old version ")
         logger.error(f"  Failed Invariant: '{new_version}' > '{old_version}'")
+        logger.error("If the invariant is from vcs tags try '--ignore-vcs-tag' option.")
         return False
     else:
         return True
 
 
 def incr_dispatch(
     old_version: str,
@@ -722,14 +723,20 @@
     is_flag=True,
     help=(
         "Commit even when working directory is has uncomitted changes. "
         "(WARNING: The commit will still be aborted if there are uncomitted "
         "to files with version strings."
     ),
 )
+@click.option(
+    "--ignore-vcs-tag",
+    default=False,
+    is_flag=True,
+    help="Ignore VCS tag invariant and update version anyway.",
+)
 @version_options
 @click.option(
     "-c",
     "--commit-message",
     default=None,
     metavar="<TMPL>",
     help="Set commit message template.",
@@ -748,14 +755,15 @@
     "--push/--no-push",
     default=None,
     help="Push to the default remote.",
 )
 def update(
     dry           : bool = False,
     allow_dirty   : bool = False,
+    ignore_vcs_tag: bool = False,
     fetch         : bool = True,
     verbose       : int = 0,
     major         : bool = False,
     minor         : bool = False,
     patch         : bool = False,
     tag           : typ.Optional[str] = None,
     tag_num       : bool = False,
@@ -782,15 +790,16 @@
 
     try:
         cfg = _parse_vcs_options(cfg, commit, tag_commit, push)
     except ValueError as ex:
         logger.warning(f"Invalid argument: {ex}")
         sys.exit(1)
 
-    cfg = _update_cfg_from_vcs(cfg, fetch)
+    if not ignore_vcs_tag:
+        cfg = _update_cfg_from_vcs(cfg, fetch)
 
     old_version = cfg.current_version
     if set_version is None:
         new_version = incr_dispatch(
             old_version,
             raw_pattern=cfg.version_pattern,
             major=major,
```

### Comparing `bumpver-2023.1121/src/bumpver/config.py` & `bumpver-2023.1122/src/bumpver/config.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/parse.py` & `bumpver-2023.1122/src/bumpver/parse.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/patterns.py` & `bumpver-2023.1122/src/bumpver/patterns.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/pysix.py` & `bumpver-2023.1122/src/bumpver/pysix.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/regexfmt.py` & `bumpver-2023.1122/src/bumpver/regexfmt.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/rewrite.py` & `bumpver-2023.1122/src/bumpver/rewrite.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/utils.py` & `bumpver-2023.1122/src/bumpver/utils.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/v1patterns.py` & `bumpver-2023.1122/src/bumpver/v1patterns.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/v1rewrite.py` & `bumpver-2023.1122/src/bumpver/v1rewrite.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/v1version.py` & `bumpver-2023.1122/src/bumpver/v1version.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/v2patterns.py` & `bumpver-2023.1122/src/bumpver/v2patterns.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/v2rewrite.py` & `bumpver-2023.1122/src/bumpver/v2rewrite.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/v2version.py` & `bumpver-2023.1122/src/bumpver/v2version.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/vcs.py` & `bumpver-2023.1122/src/bumpver/vcs.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver/version.py` & `bumpver-2023.1122/src/bumpver/version.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/src/bumpver.egg-info/PKG-INFO` & `bumpver-2023.1122/src/bumpver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpver
-Version: 2023.1121
+Version: 2023.1122
 Summary: Bump version numbers in project files.
 Home-page: https://github.com/mbarkhau/bumpver
 Author: Manuel Barkhau
 Author-email: mbarkhau@gmail.com
 License: MIT
 Keywords: version bumpver calver semver versioning bumpversion pep440
 Classifier: Development Status :: 4 - Beta
@@ -47,15 +47,15 @@
 [url_calver_org]: https://calver.org/
 
 
 Project/Repo:
 
 [![MIT License][img_license]][url_license]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
-[![CalVer 2023.1121][img_version]][url_version]
+[![CalVer 2023.1122][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![PyPI Downloads][img_downloads]][url_downloads]
 
 Code Quality/CI:
 
 [![GitHub Build Status][img_github_build]][url_github_build]
 [![GitLab Build Status][img_gitlab_build]][url_gitlab_build]
@@ -81,15 +81,15 @@
 
 [img_style]: https://img.shields.io/badge/code%20style-%20sjfmt-f71.svg
 [url_style]: https://gitlab.com/mbarkhau/straitjacket/
 
 [img_downloads]: https://pepy.tech/badge/bumpver/month
 [url_downloads]: https://pepy.tech/project/bumpver
 
-[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1121&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=CalVer&message=2023.1122&color=blue
 [url_version]: https://pypi.org/project/bumpver/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/bumpver/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/bumpver.svg
 [url_pyversions]: https://pypi.python.org/pypi/bumpver
@@ -597,16 +597,16 @@
 $ bumpver --help
 Usage: bumpver [OPTIONS] COMMAND [ARGS]...
 
   Automatically update version strings in plaintext files.
 
 Options:
   --version      Show the version and exit.
-  --help         Show this message and exit.
   -v, --verbose  Control log level. -vv for debug level.
+  -h, --help     Show this message and exit.
 
 Commands:
   grep    Search file(s) for a version pattern.
   init    Initialize [bumpver] configuration.
   show    Show current version of your project.
   test    Increment a version number for demo purposes.
   update  Update project files with the incremented version string.
@@ -619,38 +619,43 @@
 ```
 $ bumpver update --help
 Usage: bumpver update [OPTIONS]
 
   Update project files with the incremented version string.
 
 Options:
-  -d, --dry                       Display diff of changes, don't rewrite files.
+  -d, --dry                       Display diff of changes, don't rewrite
+                                  files.
   -f, --fetch / -n, --no-fetch    Sync tags from remote origin.
   -v, --verbose                   Control log level. -vv for debug level.
   --allow-dirty                   Commit even when working directory is has
-                                  uncomitted changes. (WARNING: The commit will
-                                  still be aborted if there are uncomitted to
-                                  files with version strings.
+                                  uncomitted changes. (WARNING: The commit
+                                  will still be aborted if there are
+                                  uncomitted to files with version strings.
+  --ignore-vcs-tag                Ignore VCS tag invariant and update version
+                                  anyway.
   --set-version <VERSION>         Set version explicitly.
   --date <ISODATE>                Set explicit date in format YYYY-0M-0D (e.g.
-                                  2021-05-13).
+                                  2023-05-18).
   --pin-date                      Leave date components unchanged.
   --pin-increments                Leave the auto-increments INC0 and INC1
+                                  unchanged.
   --tag-num                       Increment release tag number (rc1, rc2,
                                   rc3..).
-  -t, --tag <NAME>                Override release tag of current_version. Valid
-                                  options are: alpha, beta, dev, rc, post, final.
+  -t, --tag <NAME>                Override release tag of current_version.
+                                  Valid options are: alpha, beta, dev, rc,
+                                  post, final.
   -p, --patch                     Increment PATCH component.
   -m, --minor                     Increment MINOR component.
   --major                         Increment MAJOR component.
   -c, --commit-message <TMPL>     Set commit message template.
   --commit / --no-commit          Create a commit with all updated files.
   --tag-commit / --no-tag-commit  Tag the newly created commit.
   --push / --no-push              Push to the default remote.
-  --help                          Show this message and exit.
+  -h, --help                      Show this message and exit.
 ```
 
 <!-- END bumpver update --help -->
 
 To help with shell script automation, you can use `bumpver show --env`.
 
 ```shell
@@ -754,32 +759,32 @@
 [pep_440_normalzation_ref]: https://www.python.org/dev/peps/pep-0440/#id31
 
 
 ### Pattern Examples
 
 <!-- BEGIN pattern_examples -->
 
-|             pattern             |               examples              | PEP440 | lexico. |
-|---------------------------------|-------------------------------------|--------|---------|
-| `MAJOR.MINOR.PATCH[PYTAGNUM]`   | `0.13.10          0.16.10rc1`       | yes    | no      |
-| `MAJOR.MINOR[.PATCH[PYTAGNUM]]` | `1.11             0.3.0b5`          | yes    | no      |
-| `YYYY.BUILD[PYTAGNUM]`          | `2020.1031        2020.1148a0`      | yes    | yes     |
-| `YYYY.BUILD[-TAG]`              | `2021.1393-beta   2022.1279`        | no     | yes     |
-| `YYYY.INC0[PYTAGNUM]`           | `2020.10          2021.12b2`        | yes    | no      |
-| `YYYY0M.PATCH[-TAG]`            | `202005.12        202210.15-beta`   | no     | no¹     |
-| `YYYY0M.BUILD[-TAG]`            | `202106.1071      202106.1075-beta` | no     | yes     |
-| `YYYY.0M`                       | `2020.02          2022.09`          | no     | yes     |
-| `YYYY.MM`                       | `2020.8           2020.10`          | yes    | no      |
-| `YYYY.WW`                       | `2020.8           2021.14`          | yes    | no      |
-| `YYYY.MM.PATCH[PYTAGNUM]`       | `2020.3.12b0      2021.6.19b0`      | yes    | no      |
-| `YYYY.0M.PATCH[PYTAGNUM]`       | `2020.10.15b0     2022.07.7b0`      | no     | no¹     |
-| `YYYY.MM.INC0`                  | `2021.6.2         2022.8.9`         | yes    | no      |
-| `YYYY.MM.DD`                    | `2020.5.18        2021.8.2`         | yes    | no      |
-| `YYYY.0M.0D`                    | `2020.08.24       2022.05.03`       | no     | yes     |
-| `YY.0M.PATCH`                   | `21.04.2          21.11.12`         | no     | no²     |
+| pattern                         | examples                          | PEP440 | lexico. |
+|---------------------------------|-----------------------------------|--------|---------|
+| `MAJOR.MINOR.PATCH[PYTAGNUM]`   | `0.13.10          0.16.10`        | yes    | no      |
+| `MAJOR.MINOR[.PATCH[PYTAGNUM]]` | `0.11.15          0.16.18`        | yes    | no      |
+| `YYYY.BUILD[PYTAGNUM]`          | `2020.1031        2020.1406`      | yes    | yes     |
+| `YYYY.BUILD[-TAG]`              | `2021.1393-beta   2022.1279`      | no     | yes     |
+| `YYYY.INC0[PYTAGNUM]`           | `2020.4b0         2020.16`        | yes    | no      |
+| `YYYY0M.PATCH[-TAG]`            | `202210.10        202211.13-beta` | no     | no¹     |
+| `YYYY0M.BUILD[-TAG]`            | `202005.1269-beta 202206.1056`    | no     | yes     |
+| `YYYY.0M`                       | `2020.01          2021.04`        | no     | yes     |
+| `YYYY.MM`                       | `2020.2           2022.2`         | yes    | no      |
+| `YYYY.WW`                       | `2020.33          2020.39`        | yes    | no      |
+| `YYYY.MM.PATCH[PYTAGNUM]`       | `2022.3.1b0       2022.11.15b0`   | yes    | no      |
+| `YYYY.0M.PATCH[PYTAGNUM]`       | `2020.03.2        2022.02.4`      | no     | no¹     |
+| `YYYY.MM.INC0`                  | `2020.7.10        2021.7.7`       | yes    | no      |
+| `YYYY.MM.DD`                    | `2020.8.9         2020.8.20`      | yes    | no      |
+| `YYYY.0M.0D`                    | `2020.11.02       2022.05.03`     | no     | yes     |
+| `YY.0M.PATCH`                   | `20.05.12         22.03.5`        | no     | no²     |
 
 <!-- END pattern_examples -->
 
 - ¹ If `PATCH > 9`
 - ² For the year 2100, the part `YY` will produce 0
 
 
@@ -794,15 +799,15 @@
 If you use `VV`/`0V`, be aware that you cannot also use `YYYY`.
 Instead use `GGGG`. This is to avoid an edge case where your version
 number would run backwards if it was created around New Year.
 
 
 <!-- BEGIN weeknum_example -->
 
-```sql
+```
                    YYYY WW UU  GGGG VV
 2020-12-26 (Sat):  2020 51 51  2020 52
 2020-12-27 (Sun):  2020 51 52  2020 52
 2020-12-28 (Mon):  2020 52 52  2020 53
 2020-12-29 (Tue):  2020 52 52  2020 53
 2020-12-30 (Wed):  2020 52 52  2020 53
 2020-12-31 (Thu):  2020 52 52  2020 53
@@ -821,15 +826,15 @@
 
 The create an initial configuration for project with `bumpver init`.
 
 ```shell
 $ pip install bumpver
 ...
 Installing collected packages: click toml lexid bumpver
-Successfully installed bumpver-2023.1121
+Successfully installed bumpver-2023.1122
 
 $ cd myproject
 ~/myproject/
 
 $ bumpver init --dry
 Exiting because of '-d/--dry'. Would have written to bumpver.toml:
 
@@ -1117,14 +1122,22 @@
 |                Name                 |    role           |  since  | until |
 |-------------------------------------|-------------------|---------|-------|
 | Manuel Barkhau (mbarkhau@gmail.com) | author/maintainer | 2018-09 | -     |
 
 
 # Changelog for https://github.com/mbarkhau/bumpver
 
+## BumpVer 2023.1122
+
+- Fix [#207][gh_i207]: Add --ignore-vcs-tag for old version support purpose
+
+[gh_i207]: https://github.com/mbarkhau/bumpver/issues/207
+
+Thank you [Jusong Yu](https://github.com/unkcpz) for your contribution.
+
 ## BumpVer 2023.1121
 
 - Fix [#200][gh_i200]: Fix compatability with packaging 23.0.
 - Fix [#203][gh_i203]: Add dev to the list of valid release tags
 
 [gh_i200]: https://github.com/mbarkhau/bumpver/issues/200
 [gh_i203]: https://github.com/mbarkhau/bumpver/issues/203
```

### Comparing `bumpver-2023.1121/src/bumpver.egg-info/SOURCES.txt` & `bumpver-2023.1122/src/bumpver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/test/test_cli.py` & `bumpver-2023.1122/test/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1291,7 +1291,39 @@
 
     result = runner.invoke(cli.cli, ['update', "--patch"])
     assert result.exit_code == 0
 
     _, cfg = config.init()
     latest_version = cli.get_latest_vcs_version_tag(cfg, fetch=False)
     assert latest_version == "0.1.10"
+
+
+def test_ignore_vcs_tag(runner, monkeypatch):
+    result = runner.invoke(cli.cli, ['init', "-vv"])
+    assert result.exit_code == 0
+
+    _update_config_val("bumpver.toml", push="false")
+    _update_config_val("bumpver.toml", current_version='"0.1.8"')
+    _update_config_val("bumpver.toml", version_pattern='"MAJOR.MINOR.PATCH"')
+
+    _vcs_init("git", files=["bumpver.toml"])
+    _, cfg = config.init()
+
+    # mock latest vcs tag 0.2.0 but cfg.current_version is 0.1.8
+    monkeypatch.setattr(cli, "get_latest_vcs_version_tag", lambda cfg, fetch: "0.2.0")
+    assert cfg.current_version == "0.1.8"
+    assert cli.get_latest_vcs_version_tag(cfg, fetch=False) == "0.2.0"
+
+    result = runner.invoke(cli.cli, ['update', "--set-version", "0.1.9"])
+    assert result.exit_code == 1
+
+    result = runner.invoke(
+        cli.cli, ['update', "-vv", "--ignore-vcs-tag", "--dry", "--set-version", "0.1.9"]
+    )
+    assert result.exit_code == 0
+
+    out_lines = set(result.output.splitlines())
+    assert '-current_version = "0.1.8"' in out_lines
+    assert '+current_version = "0.1.9"' in out_lines
+
+    latest_version = cli.get_latest_vcs_version_tag(cfg, fetch=False)
+    assert latest_version == "0.2.0"
```

### Comparing `bumpver-2023.1121/test/test_config.py` & `bumpver-2023.1122/test/test_config.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/test/test_parse.py` & `bumpver-2023.1122/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/test/test_patterns.py` & `bumpver-2023.1122/test/test_patterns.py`

 * *Files identical despite different names*

### Comparing `bumpver-2023.1121/test/test_rewrite.py` & `bumpver-2023.1122/test/test_rewrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
     file_patterns   = {"src/bumpver/__init__.py": [init_pattern]}
     rewritten_datas = v1rewrite.iter_rewritten(file_patterns, new_vinfo)
     rfd             = list(rewritten_datas)[0]
     expected        = [
         "# This file is part of the bumpver project",
         "# https://github.com/mbarkhau/bumpver",
         "#",
-        "# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License",
+        "# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License",
         "# SPDX-License-Identifier: MIT",
         '"""BumpVer: A CLI program for versioning."""',
         '',
         '__version__ = "2018.0123"',
         '',
     ]
     assert rfd.new_lines == expected
@@ -252,15 +252,15 @@
 
     rewritten_datas = v2rewrite.iter_rewritten(file_patterns, new_vinfo)
     rfd             = list(rewritten_datas)[0]
     expected        = [
         "# This file is part of the bumpver project",
         "# https://github.com/mbarkhau/bumpver",
         "#",
-        "# Copyright (c) 2018-2022 Manuel Barkhau (mbarkhau@gmail.com) - MIT License",
+        "# Copyright (c) 2018-2023 Manuel Barkhau (mbarkhau@gmail.com) - MIT License",
         "# SPDX-License-Identifier: MIT",
         '"""BumpVer: A CLI program for versioning."""',
         '',
         '__version__ = "2018.0123"',
         '',
     ]
     assert rfd.new_lines == expected
```

### Comparing `bumpver-2023.1121/test/test_version.py` & `bumpver-2023.1122/test/test_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     cur_version = cur_date.strftime("v%Y%m") + ".0001-dev"
 
     monkeypatch.setattr(version, 'TODAY', cur_date)
 
     for _ in range(1000):
         cur_date += dt.timedelta(days=int((1 + random.random()) ** 10))
         new_version = v1version.incr(
-            cur_version, tag=random.choice([None, "alpha", "beta", "rc", "final", "post"])
+            cur_version, tag=random.choice([None, "dev", "alpha", "beta", "rc", "final", "post"])
         )
         assert cur_version < new_version
         cur_version = new_version
 
 
 def test_bump_tag_num():
     raw_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
@@ -259,15 +259,15 @@
     result = v2version.format_version(vinfo, raw_pattern='__version__ = "YYYY.BUILD[-TAG]"')
     assert result == '__version__ = "2007.0033-beta"'
 
     result = v2version.format_version(vinfo, raw_pattern='__version__ = "YYYY.BLD"')
     assert result == '__version__ = "2007.33"'
 
 
-WEEK_PATTERN_TEXT_CASES = [
+WEEK_PATTERN_TEST_CASES = [
     ("YYYYWW.PATCH", True),
     ("YYYYUU.PATCH", True),
     ("GGGGVV.PATCH", True),
     ("YYWW.PATCH"  , True),
     ("YYUU.PATCH"  , True),
     ("GGVV.PATCH"  , True),
     ("0YWW.PATCH"  , True),
@@ -287,10 +287,27 @@
     ("0YVV.PATCH"  , False),
     ("0G0W.PATCH"  , False),
     ("0G0U.PATCH"  , False),
     ("0Y0V.PATCH"  , False),
 ]
 
 
-@pytest.mark.parametrize("pattern, expected", WEEK_PATTERN_TEXT_CASES)
+@pytest.mark.parametrize("pattern, expected", WEEK_PATTERN_TEST_CASES)
 def test_is_valid_week_pattern(pattern, expected):
     assert v2version.is_valid_week_pattern(pattern) == expected
+
+
+PEP440_TEST_CASES = [
+    ("v2017.54321"       , "2017.54321"),
+    ("v201808.0123-alpha", "201808.123a0"),
+    ("v201811.0007-beta" , "201811.7b0"),
+    ("v2020.1003-alpha"  , "2020.1003a0"),
+    ("v2020.1003-beta"   , "2020.1003b0"),
+    ("v2020.1003-dev"    , "2020.1003.dev0"),
+    ("v2017q1.54321"     , "v2017q1.54321"),
+    ("1.2.3"             , "1.2.3"),
+]
+
+
+@pytest.mark.parametrize("version_str, expected", PEP440_TEST_CASES)
+def test_to_pep440(version_str, expected):
+    assert version.to_pep440(version_str) == expected
```

### Comparing `bumpver-2023.1121/test/util.py` & `bumpver-2023.1122/test/util.py`

 * *Files identical despite different names*

