# Comparing `tmp/u8488a-0.1.1.tar.gz` & `tmp/u8488a-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "u8488a-0.1.1.tar", last modified: Thu May 18 04:38:24 2023, max compression
+gzip compressed data, was "u8488a-0.1.2.tar", last modified: Thu May 18 16:02:54 2023, max compression
```

## Comparing `u8488a-0.1.1.tar` & `u8488a-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 agrses    (1000) agrses    (1000)        0 2023-05-18 04:38:24.722971 u8488a-0.1.1/
--rw-r--r--   0 agrses    (1000) agrses    (1000)      413 2023-05-18 04:38:24.722971 u8488a-0.1.1/PKG-INFO
--rw-r--r--   0 agrses    (1000) agrses    (1000)     1172 2023-05-18 04:23:28.000000 u8488a-0.1.1/README.md
--rw-r--r--   0 agrses    (1000) agrses    (1000)       38 2023-05-18 04:38:24.722971 u8488a-0.1.1/setup.cfg
--rw-r--r--   0 agrses    (1000) agrses    (1000)      628 2023-05-18 04:37:53.000000 u8488a-0.1.1/setup.py
-drwxr-xr-x   0 agrses    (1000) agrses    (1000)        0 2023-05-18 04:38:24.722971 u8488a-0.1.1/u8488a/
--rw-r--r--   0 agrses    (1000) agrses    (1000)        0 2023-05-18 03:57:39.000000 u8488a-0.1.1/u8488a/__init__.py
--rw-r--r--   0 agrses    (1000) agrses    (1000)     2173 2023-05-18 04:07:00.000000 u8488a-0.1.1/u8488a/base.py
--rw-r--r--   0 agrses    (1000) agrses    (1000)     1379 2023-05-18 03:58:58.000000 u8488a-0.1.1/u8488a/usrp.py
-drwxr-xr-x   0 agrses    (1000) agrses    (1000)        0 2023-05-18 04:38:24.722971 u8488a-0.1.1/u8488a.egg-info/
--rw-r--r--   0 agrses    (1000) agrses    (1000)      413 2023-05-18 04:38:24.000000 u8488a-0.1.1/u8488a.egg-info/PKG-INFO
--rw-r--r--   0 agrses    (1000) agrses    (1000)      187 2023-05-18 04:38:24.000000 u8488a-0.1.1/u8488a.egg-info/SOURCES.txt
--rw-r--r--   0 agrses    (1000) agrses    (1000)        1 2023-05-18 04:38:24.000000 u8488a-0.1.1/u8488a.egg-info/dependency_links.txt
--rw-r--r--   0 agrses    (1000) agrses    (1000)        7 2023-05-18 04:38:24.000000 u8488a-0.1.1/u8488a.egg-info/top_level.txt
+drwxr-xr-x   0 agrses    (1000) agrses    (1000)        0 2023-05-18 16:02:54.951693 u8488a-0.1.2/
+-rw-r--r--   0 agrses    (1000) agrses    (1000)     1468 2023-05-18 16:02:54.951693 u8488a-0.1.2/PKG-INFO
+-rw-r--r--   0 agrses    (1000) agrses    (1000)     1172 2023-05-18 04:23:28.000000 u8488a-0.1.2/README.md
+-rw-r--r--   0 agrses    (1000) agrses    (1000)       38 2023-05-18 16:02:54.951693 u8488a-0.1.2/setup.cfg
+-rw-r--r--   0 agrses    (1000) agrses    (1000)      663 2023-05-18 16:02:52.000000 u8488a-0.1.2/setup.py
+drwxr-xr-x   0 agrses    (1000) agrses    (1000)        0 2023-05-18 16:02:54.950693 u8488a-0.1.2/u8488a/
+-rw-r--r--   0 agrses    (1000) agrses    (1000)        0 2023-05-18 03:57:39.000000 u8488a-0.1.2/u8488a/__init__.py
+-rw-r--r--   0 agrses    (1000) agrses    (1000)     2173 2023-05-18 04:07:00.000000 u8488a-0.1.2/u8488a/base.py
+-rw-r--r--   0 agrses    (1000) agrses    (1000)     1379 2023-05-18 03:58:58.000000 u8488a-0.1.2/u8488a/usrp.py
+drwxr-xr-x   0 agrses    (1000) agrses    (1000)        0 2023-05-18 16:02:54.951693 u8488a-0.1.2/u8488a.egg-info/
+-rw-r--r--   0 agrses    (1000) agrses    (1000)     1468 2023-05-18 16:02:54.000000 u8488a-0.1.2/u8488a.egg-info/PKG-INFO
+-rw-r--r--   0 agrses    (1000) agrses    (1000)      187 2023-05-18 16:02:54.000000 u8488a-0.1.2/u8488a.egg-info/SOURCES.txt
+-rw-r--r--   0 agrses    (1000) agrses    (1000)        1 2023-05-18 16:02:54.000000 u8488a-0.1.2/u8488a.egg-info/dependency_links.txt
+-rw-r--r--   0 agrses    (1000) agrses    (1000)        7 2023-05-18 16:02:54.000000 u8488a-0.1.2/u8488a.egg-info/top_level.txt
```

### Comparing `u8488a-0.1.1/README.md` & `u8488a-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `u8488a-0.1.1/u8488a/base.py` & `u8488a-0.1.2/u8488a/base.py`

 * *Files identical despite different names*

### Comparing `u8488a-0.1.1/u8488a/usrp.py` & `u8488a-0.1.2/u8488a/usrp.py`

 * *Files identical despite different names*

