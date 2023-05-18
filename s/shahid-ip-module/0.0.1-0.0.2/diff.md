# Comparing `tmp/shahid_ip_module-0.0.1.tar.gz` & `tmp/shahid_ip_module-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shahid_ip_module-0.0.1.tar", last modified: Thu May 18 13:32:12 2023, max compression
+gzip compressed data, was "shahid_ip_module-0.0.2.tar", last modified: Thu May 18 13:33:35 2023, max compression
```

## Comparing `shahid_ip_module-0.0.1.tar` & `shahid_ip_module-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 shahid    (1000) shahid    (1000)        0 2023-05-18 13:32:12.486580 shahid_ip_module-0.0.1/
--rw-rw-r--   0 shahid    (1000) shahid    (1000)      170 2023-05-18 13:32:12.486580 shahid_ip_module-0.0.1/PKG-INFO
--rw-rw-r--   0 shahid    (1000) shahid    (1000)       38 2023-05-18 13:32:12.486580 shahid_ip_module-0.0.1/setup.cfg
--rw-rw-r--   0 shahid    (1000) shahid    (1000)      270 2023-05-18 13:31:35.000000 shahid_ip_module-0.0.1/setup.py
-drwxrwxr-x   0 shahid    (1000) shahid    (1000)        0 2023-05-18 13:32:12.486580 shahid_ip_module-0.0.1/shahid/
--rw-rw-r--   0 shahid    (1000) shahid    (1000)      485 2023-05-18 13:17:47.000000 shahid_ip_module-0.0.1/shahid/__init__.py
-drwxrwxr-x   0 shahid    (1000) shahid    (1000)        0 2023-05-18 13:32:12.486580 shahid_ip_module-0.0.1/shahid_ip_module.egg-info/
--rw-rw-r--   0 shahid    (1000) shahid    (1000)      170 2023-05-18 13:32:12.000000 shahid_ip_module-0.0.1/shahid_ip_module.egg-info/PKG-INFO
--rw-rw-r--   0 shahid    (1000) shahid    (1000)      187 2023-05-18 13:32:12.000000 shahid_ip_module-0.0.1/shahid_ip_module.egg-info/SOURCES.txt
--rw-rw-r--   0 shahid    (1000) shahid    (1000)        1 2023-05-18 13:32:12.000000 shahid_ip_module-0.0.1/shahid_ip_module.egg-info/dependency_links.txt
--rw-rw-r--   0 shahid    (1000) shahid    (1000)        7 2023-05-18 13:32:12.000000 shahid_ip_module-0.0.1/shahid_ip_module.egg-info/top_level.txt
+drwxrwxr-x   0 shahid    (1000) shahid    (1000)        0 2023-05-18 13:33:35.850141 shahid_ip_module-0.0.2/
+-rw-rw-r--   0 shahid    (1000) shahid    (1000)      170 2023-05-18 13:33:35.850141 shahid_ip_module-0.0.2/PKG-INFO
+-rw-rw-r--   0 shahid    (1000) shahid    (1000)       38 2023-05-18 13:33:35.850141 shahid_ip_module-0.0.2/setup.cfg
+-rw-rw-r--   0 shahid    (1000) shahid    (1000)      270 2023-05-18 13:33:21.000000 shahid_ip_module-0.0.2/setup.py
+drwxrwxr-x   0 shahid    (1000) shahid    (1000)        0 2023-05-18 13:33:35.850141 shahid_ip_module-0.0.2/shahid/
+-rw-rw-r--   0 shahid    (1000) shahid    (1000)      485 2023-05-18 13:17:47.000000 shahid_ip_module-0.0.2/shahid/__init__.py
+drwxrwxr-x   0 shahid    (1000) shahid    (1000)        0 2023-05-18 13:33:35.850141 shahid_ip_module-0.0.2/shahid_ip_module.egg-info/
+-rw-rw-r--   0 shahid    (1000) shahid    (1000)      170 2023-05-18 13:33:35.000000 shahid_ip_module-0.0.2/shahid_ip_module.egg-info/PKG-INFO
+-rw-rw-r--   0 shahid    (1000) shahid    (1000)      187 2023-05-18 13:33:35.000000 shahid_ip_module-0.0.2/shahid_ip_module.egg-info/SOURCES.txt
+-rw-rw-r--   0 shahid    (1000) shahid    (1000)        1 2023-05-18 13:33:35.000000 shahid_ip_module-0.0.2/shahid_ip_module.egg-info/dependency_links.txt
+-rw-rw-r--   0 shahid    (1000) shahid    (1000)        7 2023-05-18 13:33:35.000000 shahid_ip_module-0.0.2/shahid_ip_module.egg-info/top_level.txt
```

