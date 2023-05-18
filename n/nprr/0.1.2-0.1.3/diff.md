# Comparing `tmp/nprr-0.1.2.tar.gz` & `tmp/nprr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nprr-0.1.2.tar", last modified: Thu May 18 05:57:26 2023, max compression
+gzip compressed data, was "nprr-0.1.3.tar", last modified: Thu May 18 06:05:45 2023, max compression
```

## Comparing `nprr-0.1.2.tar` & `nprr-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:57:26.799394 nprr-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-18 05:57:19.000000 nprr-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-18 05:57:26.799394 nprr-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-18 05:57:19.000000 nprr-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:57:26.795393 nprr-0.1.2/nprr/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 05:57:19.000000 nprr-0.1.2/nprr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-18 05:57:19.000000 nprr-0.1.2/nprr/cgf.py
--rw-r--r--   0 runner    (1001) docker     (123)    29740 2023-05-18 05:57:19.000000 nprr-0.1.2/nprr/dpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-18 05:57:19.000000 nprr-0.1.2/nprr/mechanisms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-18 05:57:19.000000 nprr-0.1.2/nprr/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 05:57:19.000000 nprr-0.1.2/nprr/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:57:26.799394 nprr-0.1.2/nprr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-18 05:57:26.000000 nprr-0.1.2/nprr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-18 05:57:26.000000 nprr-0.1.2/nprr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:57:26.000000 nprr-0.1.2/nprr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:57:26.000000 nprr-0.1.2/nprr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 05:57:26.000000 nprr-0.1.2/nprr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 05:57:26.000000 nprr-0.1.2/nprr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-18 05:57:19.000000 nprr-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 05:57:26.799394 nprr-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-18 05:57:19.000000 nprr-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:05:45.019311 nprr-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-18 06:05:37.000000 nprr-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-18 06:05:45.019311 nprr-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-18 06:05:37.000000 nprr-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:05:45.019311 nprr-0.1.3/nprr/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/cgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29740 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/dpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/mechanisms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:05:45.019311 nprr-0.1.3/nprr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-18 06:05:45.000000 nprr-0.1.3/nprr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-18 06:05:45.000000 nprr-0.1.3/nprr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:05:45.000000 nprr-0.1.3/nprr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:05:44.000000 nprr-0.1.3/nprr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 06:05:45.000000 nprr-0.1.3/nprr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 06:05:45.000000 nprr-0.1.3/nprr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-18 06:05:37.000000 nprr-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:05:45.019311 nprr-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-18 06:05:37.000000 nprr-0.1.3/setup.py
```

### Comparing `nprr-0.1.2/LICENSE` & `nprr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nprr-0.1.2/README.md` & `nprr-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nprr-0.1.2/nprr/cgf.py` & `nprr-0.1.3/nprr/cgf.py`

 * *Files identical despite different names*

### Comparing `nprr-0.1.2/nprr/dpcs.py` & `nprr-0.1.3/nprr/dpcs.py`

 * *Files identical despite different names*

### Comparing `nprr-0.1.2/nprr/mechanisms.py` & `nprr-0.1.3/nprr/mechanisms.py`

 * *Files identical despite different names*

### Comparing `nprr-0.1.2/nprr/plotting.py` & `nprr-0.1.3/nprr/plotting.py`

 * *Files identical despite different names*

