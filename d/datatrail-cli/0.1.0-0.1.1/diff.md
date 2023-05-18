# Comparing `tmp/datatrail_cli-0.1.0.tar.gz` & `tmp/datatrail_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrail_cli-0.1.0.tar", max compression
+gzip compressed data, was "datatrail_cli-0.1.1.tar", max compression
```

## Comparing `datatrail_cli-0.1.0.tar` & `datatrail_cli-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0     1080 2023-05-02 18:30:49.351906 datatrail_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0       21 2023-05-03 15:52:40.389860 datatrail_cli-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-02 18:33:06.259345 datatrail_cli-0.1.0/dtcli/__init__.py
--rw-r--r--   0        0        0      759 2023-05-03 18:42:09.477323 datatrail_cli-0.1.0/dtcli/cli.py
--rw-r--r--   0        0        0      166 2023-05-03 18:07:57.558924 datatrail_cli-0.1.0/dtcli/ls.py
--rw-r--r--   0        0        0      249 2023-05-03 18:07:36.317194 datatrail_cli-0.1.0/dtcli/ps.py
--rw-r--r--   0        0        0      583 2023-05-03 18:07:13.786239 datatrail_cli-0.1.0/dtcli/pull.py
--rw-r--r--   0        0        0      493 2023-05-03 15:36:32.037215 datatrail_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 datatrail_cli-0.1.0/setup.py
--rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 datatrail_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-18 15:48:29.519183 datatrail_cli-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3492 2023-05-18 15:48:29.519183 datatrail_cli-0.1.1/README.md
+-rw-r--r--   0        0        0      214 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/__init__.py
+-rw-r--r--   0        0        0      893 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/cli.py
+-rw-r--r--   0        0        0     3713 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/config.py
+-rw-r--r--   0        0        0     1062 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/config.yaml
+-rw-r--r--   0        0        0     3283 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/ls.py
+-rw-r--r--   0        0        0     4091 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/ps.py
+-rw-r--r--   0        0        0     3576 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/pull.py
+-rw-r--r--   0        0        0     8674 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/src/functions.py
+-rw-r--r--   0        0        0     8262 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/utilities/cadcclient.py
+-rw-r--r--   0        0        0     1151 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/dtcli/utilities/utilities.py
+-rw-r--r--   0        0        0     1048 2023-05-18 15:48:29.527183 datatrail_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 datatrail_cli-0.1.1/PKG-INFO
```

### Comparing `datatrail_cli-0.1.0/LICENSE` & `datatrail_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

