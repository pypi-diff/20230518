# Comparing `tmp/gitea-backup-2.0.1.tar.gz` & `tmp/gitea-backup-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitea-backup-2.0.1.tar", last modified: Thu May 18 03:04:34 2023, max compression
+gzip compressed data, was "gitea-backup-2.0.2.tar", last modified: Thu May 18 03:05:53 2023, max compression
```

## Comparing `gitea-backup-2.0.1.tar` & `gitea-backup-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:04:34.061404 gitea-backup-2.0.1/
--rw-r--r--   0 noursofanati   (501) staff       (20)    34694 2023-05-18 03:04:31.000000 gitea-backup-2.0.1/CHANGES.rst
--rw-r--r--   0 noursofanati   (501) staff       (20)     1085 2023-05-17 22:46:58.000000 gitea-backup-2.0.1/LICENSE.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)       28 2023-05-17 22:46:58.000000 gitea-backup-2.0.1/MANIFEST.in
--rw-r--r--   0 noursofanati   (501) staff       (20)     9397 2023-05-18 03:04:34.061287 gitea-backup-2.0.1/PKG-INFO
--rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-18 03:04:33.000000 gitea-backup-2.0.1/README
--rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-18 03:04:30.000000 gitea-backup-2.0.1/README.rst
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:04:34.059759 gitea-backup-2.0.1/bin/
--rwxr-xr-x   0 noursofanati   (501) staff       (20)     1324 2023-05-18 01:08:46.000000 gitea-backup-2.0.1/bin/gitea-backup
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:04:34.060063 gitea-backup-2.0.1/gitea_backup/
--rw-------   0 noursofanati   (501) staff       (20)       22 2023-05-18 03:04:30.000000 gitea-backup-2.0.1/gitea_backup/__init__.py
--rw-r--r--   0 noursofanati   (501) staff       (20)    47182 2023-05-18 02:38:47.000000 gitea-backup-2.0.1/gitea_backup/gitea_backup.py
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:04:34.061026 gitea-backup-2.0.1/gitea_backup.egg-info/
--rw-r--r--   0 noursofanati   (501) staff       (20)     9397 2023-05-18 03:04:34.000000 gitea-backup-2.0.1/gitea_backup.egg-info/PKG-INFO
--rw-r--r--   0 noursofanati   (501) staff       (20)      325 2023-05-18 03:04:34.000000 gitea-backup-2.0.1/gitea_backup.egg-info/SOURCES.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-18 03:04:34.000000 gitea-backup-2.0.1/gitea_backup.egg-info/dependency_links.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)       13 2023-05-18 03:04:34.000000 gitea-backup-2.0.1/gitea_backup.egg-info/top_level.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-18 03:04:34.000000 gitea-backup-2.0.1/gitea_backup.egg-info/zip-safe
--rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-17 22:46:58.000000 gitea-backup-2.0.1/requirements.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)       38 2023-05-18 03:04:34.061442 gitea-backup-2.0.1/setup.cfg
--rw-r--r--   0 noursofanati   (501) staff       (20)     1563 2023-05-18 03:02:20.000000 gitea-backup-2.0.1/setup.py
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:05:53.105106 gitea-backup-2.0.2/
+-rw-r--r--   0 noursofanati   (501) staff       (20)    34835 2023-05-18 03:05:50.000000 gitea-backup-2.0.2/CHANGES.rst
+-rw-r--r--   0 noursofanati   (501) staff       (20)     1085 2023-05-17 22:46:58.000000 gitea-backup-2.0.2/LICENSE.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)       28 2023-05-17 22:46:58.000000 gitea-backup-2.0.2/MANIFEST.in
+-rw-r--r--   0 noursofanati   (501) staff       (20)     9397 2023-05-18 03:05:53.104991 gitea-backup-2.0.2/PKG-INFO
+-rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-18 03:05:52.000000 gitea-backup-2.0.2/README
+-rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-18 03:05:49.000000 gitea-backup-2.0.2/README.rst
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:05:53.102908 gitea-backup-2.0.2/bin/
+-rwxr-xr-x   0 noursofanati   (501) staff       (20)     1322 2023-05-18 03:05:32.000000 gitea-backup-2.0.2/bin/gitea-backup
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:05:53.103267 gitea-backup-2.0.2/gitea_backup/
+-rw-------   0 noursofanati   (501) staff       (20)       22 2023-05-18 03:05:49.000000 gitea-backup-2.0.2/gitea_backup/__init__.py
+-rw-r--r--   0 noursofanati   (501) staff       (20)    47182 2023-05-18 02:38:47.000000 gitea-backup-2.0.2/gitea_backup/gitea_backup.py
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-18 03:05:53.104601 gitea-backup-2.0.2/gitea_backup.egg-info/
+-rw-r--r--   0 noursofanati   (501) staff       (20)     9397 2023-05-18 03:05:53.000000 gitea-backup-2.0.2/gitea_backup.egg-info/PKG-INFO
+-rw-r--r--   0 noursofanati   (501) staff       (20)      325 2023-05-18 03:05:53.000000 gitea-backup-2.0.2/gitea_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-18 03:05:53.000000 gitea-backup-2.0.2/gitea_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)       13 2023-05-18 03:05:53.000000 gitea-backup-2.0.2/gitea_backup.egg-info/top_level.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-18 03:04:34.000000 gitea-backup-2.0.2/gitea_backup.egg-info/zip-safe
+-rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-17 22:46:58.000000 gitea-backup-2.0.2/requirements.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)       38 2023-05-18 03:05:53.105141 gitea-backup-2.0.2/setup.cfg
+-rw-r--r--   0 noursofanati   (501) staff       (20)     1563 2023-05-18 03:02:20.000000 gitea-backup-2.0.2/setup.py
```

### Comparing `gitea-backup-2.0.1/CHANGES.rst` & `gitea-backup-2.0.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 Changelog
 =========
 
+2.0.2 (2023-05-18)
+------------------
+------------
+- Rename. [Nour Sofanati]
+
+
 2.0.1 (2023-05-18)
 ------------------
+- Release version 2.0.1. [Nour Sofanati]
+
+
+2.0.0 (2023-05-18)
 ------------------
 - Release version 2.0.0. [Nour Sofanati]
 
 
 1.0.0 (2023-05-18)
 ------------------
 - Release version 1.0.0. [Nour Sofanati]
```

### Comparing `gitea-backup-2.0.1/LICENSE.txt` & `gitea-backup-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.0.1/PKG-INFO` & `gitea-backup-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitea-backup
-Version: 2.0.1
+Version: 2.0.2
 Summary: backup a gitea user or organization
 Home-page: http://github.com/noursofanati/python-gitea-backup
 Author: Nour Sofanati
 Author-email: nour@simplebackups.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: System :: Archiving :: Backup
```

### Comparing `gitea-backup-2.0.1/README` & `gitea-backup-2.0.2/README`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.0.1/README.rst` & `gitea-backup-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.0.1/bin/gitea-backup` & `gitea-backup-2.0.2/bin/gitea-backup`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import os, sys, logging
 
-from github_backup.github_backup import (
+from gitea_backup.gitea_backup import (
     backup_account,
     backup_repositories,
     check_git_lfs_install,
     filter_repositories,
     get_authenticated_user,
     log_info,
     log_warning,
```

### Comparing `gitea-backup-2.0.1/gitea_backup/gitea_backup.py` & `gitea-backup-2.0.2/gitea_backup/gitea_backup.py`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.0.1/gitea_backup.egg-info/PKG-INFO` & `gitea-backup-2.0.2/gitea_backup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitea-backup
-Version: 2.0.1
+Version: 2.0.2
 Summary: backup a gitea user or organization
 Home-page: http://github.com/noursofanati/python-gitea-backup
 Author: Nour Sofanati
 Author-email: nour@simplebackups.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: System :: Archiving :: Backup
```

### Comparing `gitea-backup-2.0.1/setup.py` & `gitea-backup-2.0.2/setup.py`

 * *Files identical despite different names*

