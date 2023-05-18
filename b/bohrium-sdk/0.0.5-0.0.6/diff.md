# Comparing `tmp/bohrium-sdk-0.0.5.tar.gz` & `tmp/bohrium-sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.0.5.tar", last modified: Thu May 18 03:21:47 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.0.6.tar", last modified: Thu May 18 03:23:25 2023, max compression
```

## Comparing `bohrium-sdk-0.0.5.tar` & `bohrium-sdk-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-18 03:21:47.321310 bohrium-sdk-0.0.5/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-18 03:21:47.320928 bohrium-sdk-0.0.5/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.0.5/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-18 03:21:47.318924 bohrium-sdk-0.0.5/bohrium-sdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.0.5/bohrium-sdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4232 2023-05-18 03:20:07.000000 bohrium-sdk-0.0.5/bohrium-sdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:16.000000 bohrium-sdk-0.0.5/bohrium-sdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:13.000000 bohrium-sdk-0.0.5/bohrium-sdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:16:57.000000 bohrium-sdk-0.0.5/bohrium-sdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:51.000000 bohrium-sdk-0.0.5/bohrium-sdk/project.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-18 03:21:47.320535 bohrium-sdk-0.0.5/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-18 03:21:47.000000 bohrium-sdk-0.0.5/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      325 2023-05-18 03:21:47.000000 bohrium-sdk-0.0.5/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-18 03:21:47.000000 bohrium-sdk-0.0.5/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-18 03:21:47.000000 bohrium-sdk-0.0.5/bohrium_sdk.egg-info/entry_points.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       12 2023-05-18 03:21:47.000000 bohrium-sdk-0.0.5/bohrium_sdk.egg-info/top_level.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-18 03:21:47.321383 bohrium-sdk-0.0.5/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      499 2023-05-18 03:21:31.000000 bohrium-sdk-0.0.5/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-18 03:23:25.324065 bohrium-sdk-0.0.6/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-18 03:23:25.323440 bohrium-sdk-0.0.6/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.0.6/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-18 03:23:25.320198 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-18 03:23:25.000000 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      295 2023-05-18 03:23:25.000000 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-18 03:23:25.000000 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-18 03:23:25.000000 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        7 2023-05-18 03:23:25.000000 bohrium-sdk-0.0.6/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-18 03:23:25.323080 bohrium-sdk-0.0.6/brmsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.0.6/brmsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4232 2023-05-18 03:20:07.000000 bohrium-sdk-0.0.6/brmsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:16.000000 bohrium-sdk-0.0.6/brmsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:13.000000 bohrium-sdk-0.0.6/brmsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:16:57.000000 bohrium-sdk-0.0.6/brmsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:51.000000 bohrium-sdk-0.0.6/brmsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-18 03:23:25.324160 bohrium-sdk-0.0.6/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      499 2023-05-18 03:23:22.000000 bohrium-sdk-0.0.6/setup.py
```

### Comparing `bohrium-sdk-0.0.5/bohrium-sdk/client.py` & `bohrium-sdk-0.0.6/brmsdk/client.py`

 * *Files identical despite different names*

