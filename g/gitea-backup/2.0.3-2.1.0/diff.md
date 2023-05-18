# Comparing `tmp/gitea-backup-2.0.3.tar.gz` & `tmp/gitea-backup-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitea-backup-2.0.3.tar", last modified: Thu May 18 03:36:27 2023, max compression
+gzip compressed data, was "gitea-backup-2.1.0.tar", last modified: Thu May 18 03:39:23 2023, max compression
```

## Comparing `gitea-backup-2.0.3.tar` & `gitea-backup-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:36:27.959944 gitea-backup-2.0.3/
--rw-r--r--   0 noursofanati   (501) staff       (20)    34951 2023-05-18 03:36:25.000000 gitea-backup-2.0.3/CHANGES.rst
--rw-r--r--   0 noursofanati   (501) staff       (20)     1085 2023-05-17 22:46:58.000000 gitea-backup-2.0.3/LICENSE.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)       28 2023-05-17 22:46:58.000000 gitea-backup-2.0.3/MANIFEST.in
--rw-r--r--   0 noursofanati   (501) staff       (20)     9397 2023-05-18 03:36:27.959799 gitea-backup-2.0.3/PKG-INFO
--rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-18 03:36:27.000000 gitea-backup-2.0.3/README
--rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-18 03:36:24.000000 gitea-backup-2.0.3/README.rst
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:36:27.958032 gitea-backup-2.0.3/bin/
--rwxr-xr-x   0 noursofanati   (501) staff       (20)     1322 2023-05-18 03:05:32.000000 gitea-backup-2.0.3/bin/gitea-backup
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:36:27.958394 gitea-backup-2.0.3/gitea_backup/
--rw-------   0 noursofanati   (501) staff       (20)       22 2023-05-18 03:36:24.000000 gitea-backup-2.0.3/gitea_backup/__init__.py
--rw-r--r--   0 noursofanati   (501) staff       (20)    47181 2023-05-18 03:35:39.000000 gitea-backup-2.0.3/gitea_backup/gitea_backup.py
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:36:27.959441 gitea-backup-2.0.3/gitea_backup.egg-info/
--rw-r--r--   0 noursofanati   (501) staff       (20)     9397 2023-05-18 03:36:27.000000 gitea-backup-2.0.3/gitea_backup.egg-info/PKG-INFO
--rw-r--r--   0 noursofanati   (501) staff       (20)      325 2023-05-18 03:36:27.000000 gitea-backup-2.0.3/gitea_backup.egg-info/SOURCES.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-18 03:36:27.000000 gitea-backup-2.0.3/gitea_backup.egg-info/dependency_links.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)       13 2023-05-18 03:36:27.000000 gitea-backup-2.0.3/gitea_backup.egg-info/top_level.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-18 03:04:34.000000 gitea-backup-2.0.3/gitea_backup.egg-info/zip-safe
--rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-17 22:46:58.000000 gitea-backup-2.0.3/requirements.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)       38 2023-05-18 03:36:27.959991 gitea-backup-2.0.3/setup.cfg
--rw-r--r--   0 noursofanati   (501) staff       (20)     1563 2023-05-18 03:02:20.000000 gitea-backup-2.0.3/setup.py
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:39:23.451665 gitea-backup-2.1.0/
+-rw-r--r--   0 noursofanati   (501) staff       (20)    34998 2023-05-18 03:39:20.000000 gitea-backup-2.1.0/CHANGES.rst
+-rw-r--r--   0 noursofanati   (501) staff       (20)     1085 2023-05-17 22:46:58.000000 gitea-backup-2.1.0/LICENSE.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)       28 2023-05-17 22:46:58.000000 gitea-backup-2.1.0/MANIFEST.in
+-rw-r--r--   0 noursofanati   (501) staff       (20)     9397 2023-05-18 03:39:23.451536 gitea-backup-2.1.0/PKG-INFO
+-rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-18 03:39:23.000000 gitea-backup-2.1.0/README
+-rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-18 03:39:19.000000 gitea-backup-2.1.0/README.rst
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:39:23.449784 gitea-backup-2.1.0/bin/
+-rwxr-xr-x   0 noursofanati   (501) staff       (20)     1322 2023-05-18 03:05:32.000000 gitea-backup-2.1.0/bin/gitea-backup
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:39:23.450148 gitea-backup-2.1.0/gitea_backup/
+-rw-------   0 noursofanati   (501) staff       (20)       22 2023-05-18 03:39:19.000000 gitea-backup-2.1.0/gitea_backup/__init__.py
+-rw-r--r--   0 noursofanati   (501) staff       (20)    47181 2023-05-18 03:35:39.000000 gitea-backup-2.1.0/gitea_backup/gitea_backup.py
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:39:23.451174 gitea-backup-2.1.0/gitea_backup.egg-info/
+-rw-r--r--   0 noursofanati   (501) staff       (20)     9397 2023-05-18 03:39:23.000000 gitea-backup-2.1.0/gitea_backup.egg-info/PKG-INFO
+-rw-r--r--   0 noursofanati   (501) staff       (20)      325 2023-05-18 03:39:23.000000 gitea-backup-2.1.0/gitea_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-18 03:39:23.000000 gitea-backup-2.1.0/gitea_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)       13 2023-05-18 03:39:23.000000 gitea-backup-2.1.0/gitea_backup.egg-info/top_level.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-18 03:04:34.000000 gitea-backup-2.1.0/gitea_backup.egg-info/zip-safe
+-rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-17 22:46:58.000000 gitea-backup-2.1.0/requirements.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)       38 2023-05-18 03:39:23.451718 gitea-backup-2.1.0/setup.cfg
+-rw-r--r--   0 noursofanati   (501) staff       (20)     1563 2023-05-18 03:02:20.000000 gitea-backup-2.1.0/setup.py
```

### Comparing `gitea-backup-2.0.3/CHANGES.rst` & `gitea-backup-2.1.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Changelog
 =========
 
-2.0.3 (2023-05-18)
+2.1.0 (2023-05-18)
 ------------------
-------------
+------------------
+- Release version 2.0.3. [Nour Sofanati]
 - SSL Certificate. [Nour Sofanati]
 
 
 2.0.2 (2023-05-18)
 ------------------
 - Release version 2.0.2. [Nour Sofanati]
 - Rename. [Nour Sofanati]
```

### Comparing `gitea-backup-2.0.3/LICENSE.txt` & `gitea-backup-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.0.3/PKG-INFO` & `gitea-backup-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitea-backup
-Version: 2.0.3
+Version: 2.1.0
 Summary: backup a gitea user or organization
 Home-page: http://github.com/noursofanati/python-gitea-backup
 Author: Nour Sofanati
 Author-email: nour@simplebackups.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: System :: Archiving :: Backup
```

### Comparing `gitea-backup-2.0.3/README` & `gitea-backup-2.1.0/README`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.0.3/README.rst` & `gitea-backup-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.0.3/bin/gitea-backup` & `gitea-backup-2.1.0/bin/gitea-backup`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.0.3/gitea_backup/gitea_backup.py` & `gitea-backup-2.1.0/gitea_backup/gitea_backup.py`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.0.3/gitea_backup.egg-info/PKG-INFO` & `gitea-backup-2.1.0/gitea_backup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitea-backup
-Version: 2.0.3
+Version: 2.1.0
 Summary: backup a gitea user or organization
 Home-page: http://github.com/noursofanati/python-gitea-backup
 Author: Nour Sofanati
 Author-email: nour@simplebackups.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: System :: Archiving :: Backup
```

### Comparing `gitea-backup-2.0.3/setup.py` & `gitea-backup-2.1.0/setup.py`

 * *Files identical despite different names*

