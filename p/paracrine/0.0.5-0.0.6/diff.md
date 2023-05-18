# Comparing `tmp/paracrine-0.0.5.tar.gz` & `tmp/paracrine-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paracrine-0.0.5.tar", last modified: Thu May 18 11:20:32 2023, max compression
+gzip compressed data, was "paracrine-0.0.6.tar", last modified: Thu May 18 21:04:32 2023, max compression
```

## Comparing `paracrine-0.0.5.tar` & `paracrine-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 11:20:32.046545 paracrine-0.0.5/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)    34520 2023-01-20 15:32:39.000000 paracrine-0.0.5/LICENSE
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       30 2023-01-21 23:59:01.000000 paracrine-0.0.5/MANIFEST.in
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3588 2023-05-18 11:20:32.046545 paracrine-0.0.5/PKG-INFO
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3062 2023-01-29 20:33:16.000000 paracrine-0.0.5/README.md
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 11:20:32.042545 paracrine-0.0.5/paracrine/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4762 2023-01-29 17:58:35.000000 paracrine-0.0.5/paracrine/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      820 2023-01-28 23:21:08.000000 paracrine-0.0.5/paracrine/aws.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3817 2023-05-18 09:57:23.000000 paracrine-0.0.5/paracrine/certs.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     5795 2023-05-15 10:59:07.000000 paracrine-0.0.5/paracrine/config.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2362 2023-05-12 12:30:29.000000 paracrine-0.0.5/paracrine/core.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1171 2023-05-17 22:09:32.000000 paracrine-0.0.5/paracrine/cron.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3341 2023-05-14 10:12:09.000000 paracrine-0.0.5/paracrine/debian.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1856 2023-05-12 12:21:05.000000 paracrine-0.0.5/paracrine/deps.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     9937 2023-05-15 10:29:25.000000 paracrine-0.0.5/paracrine/fs.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      960 2023-02-04 16:56:52.000000 paracrine-0.0.5/paracrine/login.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      896 2023-05-15 10:59:42.000000 paracrine-0.0.5/paracrine/network.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      412 2023-01-22 00:10:48.000000 paracrine-0.0.5/paracrine/python.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      409 2023-01-28 23:21:08.000000 paracrine-0.0.5/paracrine/reboot.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3576 2023-05-12 12:35:38.000000 paracrine-0.0.5/paracrine/runner.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 11:20:32.042545 paracrine-0.0.5/paracrine/services/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-01-25 00:04:12.000000 paracrine-0.0.5/paracrine/services/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4562 2023-05-18 11:17:33.000000 paracrine-0.0.5/paracrine/services/cockroachdb.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      177 2023-05-09 13:05:32.000000 paracrine-0.0.5/paracrine/services/ntp.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4136 2023-05-14 10:11:08.000000 paracrine-0.0.5/paracrine/services/pleroma.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1247 2023-05-14 10:14:42.000000 paracrine-0.0.5/paracrine/services/postgresql.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4434 2023-05-15 10:24:12.000000 paracrine-0.0.5/paracrine/services/wireguard.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      108 2023-02-04 16:56:52.000000 paracrine-0.0.5/paracrine/setup.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2382 2023-05-14 10:17:17.000000 paracrine-0.0.5/paracrine/systemd.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 11:20:32.042545 paracrine-0.0.5/paracrine/templates/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       79 2023-01-20 15:21:51.000000 paracrine-0.0.5/paracrine/templates/certbot_requirements.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      503 2023-05-17 22:16:40.000000 paracrine-0.0.5/paracrine/templates/cockroach.service.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1774 2023-02-04 15:56:26.000000 paracrine-0.0.5/paracrine/templates/config.exs.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      121 2023-04-19 23:19:20.000000 paracrine-0.0.5/paracrine/templates/cron.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2716 2023-01-25 00:18:54.000000 paracrine-0.0.5/paracrine/templates/pleroma.nginx.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       24 2023-01-25 00:18:56.000000 paracrine-0.0.5/paracrine/templates/robots.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      300 2023-01-25 00:18:53.000000 paracrine-0.0.5/paracrine/templates/setup_db.psql.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      260 2023-01-28 23:21:08.000000 paracrine-0.0.5/paracrine/templates/wg.conf.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1180 2023-01-28 23:21:08.000000 paracrine-0.0.5/paracrine/users.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 11:20:32.042545 paracrine-0.0.5/paracrine.egg-info/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3588 2023-05-18 11:20:32.000000 paracrine-0.0.5/paracrine.egg-info/PKG-INFO
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1023 2023-05-18 11:20:32.000000 paracrine-0.0.5/paracrine.egg-info/SOURCES.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        1 2023-05-18 11:20:32.000000 paracrine-0.0.5/paracrine.egg-info/dependency_links.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       36 2023-05-18 11:20:32.000000 paracrine-0.0.5/paracrine.egg-info/requires.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       10 2023-05-18 11:20:32.000000 paracrine-0.0.5/paracrine.egg-info/top_level.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      741 2023-05-18 11:19:59.000000 paracrine-0.0.5/pyproject.toml
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       38 2023-05-18 11:20:32.046545 paracrine-0.0.5/setup.cfg
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 11:20:32.042545 paracrine-0.0.5/tests/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      835 2023-01-28 23:21:08.000000 paracrine-0.0.5/tests/test_ssh.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)    34520 2023-01-20 15:32:39.000000 paracrine-0.0.6/LICENSE
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       30 2023-01-21 23:59:01.000000 paracrine-0.0.6/MANIFEST.in
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3588 2023-05-18 21:04:32.432836 paracrine-0.0.6/PKG-INFO
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3062 2023-01-29 20:33:16.000000 paracrine-0.0.6/README.md
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/paracrine/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4762 2023-01-29 17:58:35.000000 paracrine-0.0.6/paracrine/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      820 2023-01-28 23:21:08.000000 paracrine-0.0.6/paracrine/aws.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3817 2023-05-18 09:57:23.000000 paracrine-0.0.6/paracrine/certs.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     5795 2023-05-15 10:59:07.000000 paracrine-0.0.6/paracrine/config.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2362 2023-05-12 12:30:29.000000 paracrine-0.0.6/paracrine/core.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1171 2023-05-17 22:09:32.000000 paracrine-0.0.6/paracrine/cron.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3341 2023-05-14 10:12:09.000000 paracrine-0.0.6/paracrine/debian.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1856 2023-05-12 12:21:05.000000 paracrine-0.0.6/paracrine/deps.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)    10055 2023-05-18 21:00:30.000000 paracrine-0.0.6/paracrine/fs.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      960 2023-02-04 16:56:52.000000 paracrine-0.0.6/paracrine/login.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      896 2023-05-15 10:59:42.000000 paracrine-0.0.6/paracrine/network.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      412 2023-01-22 00:10:48.000000 paracrine-0.0.6/paracrine/python.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      409 2023-01-28 23:21:08.000000 paracrine-0.0.6/paracrine/reboot.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3576 2023-05-12 12:35:38.000000 paracrine-0.0.6/paracrine/runner.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/paracrine/services/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-01-25 00:04:12.000000 paracrine-0.0.6/paracrine/services/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4961 2023-05-18 21:00:30.000000 paracrine-0.0.6/paracrine/services/cockroachdb.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      177 2023-05-09 13:05:32.000000 paracrine-0.0.6/paracrine/services/ntp.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4136 2023-05-14 10:11:08.000000 paracrine-0.0.6/paracrine/services/pleroma.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1247 2023-05-14 10:14:42.000000 paracrine-0.0.6/paracrine/services/postgresql.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4434 2023-05-15 10:24:12.000000 paracrine-0.0.6/paracrine/services/wireguard.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      108 2023-02-04 16:56:52.000000 paracrine-0.0.6/paracrine/setup.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2382 2023-05-14 10:17:17.000000 paracrine-0.0.6/paracrine/systemd.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/paracrine/templates/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       79 2023-01-20 15:21:51.000000 paracrine-0.0.6/paracrine/templates/certbot_requirements.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      503 2023-05-17 22:16:40.000000 paracrine-0.0.6/paracrine/templates/cockroach.service.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1774 2023-02-04 15:56:26.000000 paracrine-0.0.6/paracrine/templates/config.exs.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      121 2023-04-19 23:19:20.000000 paracrine-0.0.6/paracrine/templates/cron.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2716 2023-01-25 00:18:54.000000 paracrine-0.0.6/paracrine/templates/pleroma.nginx.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       24 2023-01-25 00:18:56.000000 paracrine-0.0.6/paracrine/templates/robots.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      300 2023-01-25 00:18:53.000000 paracrine-0.0.6/paracrine/templates/setup_db.psql.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      260 2023-01-28 23:21:08.000000 paracrine-0.0.6/paracrine/templates/wg.conf.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1180 2023-01-28 23:21:08.000000 paracrine-0.0.6/paracrine/users.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/paracrine.egg-info/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3588 2023-05-18 21:04:32.000000 paracrine-0.0.6/paracrine.egg-info/PKG-INFO
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1023 2023-05-18 21:04:32.000000 paracrine-0.0.6/paracrine.egg-info/SOURCES.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        1 2023-05-18 21:04:32.000000 paracrine-0.0.6/paracrine.egg-info/dependency_links.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       36 2023-05-18 21:04:32.000000 paracrine-0.0.6/paracrine.egg-info/requires.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       10 2023-05-18 21:04:32.000000 paracrine-0.0.6/paracrine.egg-info/top_level.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      741 2023-05-18 21:04:06.000000 paracrine-0.0.6/pyproject.toml
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       38 2023-05-18 21:04:32.432836 paracrine-0.0.6/setup.cfg
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-18 21:04:32.432836 paracrine-0.0.6/tests/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      835 2023-01-28 23:21:08.000000 paracrine-0.0.6/tests/test_ssh.py
```

### Comparing `paracrine-0.0.5/LICENSE` & `paracrine-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/PKG-INFO` & `paracrine-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracrine
-Version: 0.0.5
+Version: 0.0.6
 Summary: A system deployment tool
 Author-email: Tom Parker-Shemilt <palfrey@tevp.net>
 Project-URL: Homepage, https://github.com/palfrey/paracrine
 Project-URL: Bug Tracker, https://github.com/palfrey/paracrine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `paracrine-0.0.5/README.md` & `paracrine-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/__init__.py` & `paracrine-0.0.6/paracrine/__init__.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/aws.py` & `paracrine-0.0.6/paracrine/aws.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/certs.py` & `paracrine-0.0.6/paracrine/certs.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/config.py` & `paracrine-0.0.6/paracrine/config.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/core.py` & `paracrine-0.0.6/paracrine/core.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/cron.py` & `paracrine-0.0.6/paracrine/cron.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/debian.py` & `paracrine-0.0.6/paracrine/debian.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/deps.py` & `paracrine-0.0.6/paracrine/deps.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/fs.py` & `paracrine-0.0.6/paracrine/fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import pwd
 import re
 import stat
 import subprocess
 from datetime import datetime
 from difflib import unified_diff
+from pathlib import Path
 from typing import List, Optional, Union
 
 from .config import data_files, jinja_env
 
 
 def hash_data(data: bytes) -> str:
     m = hashlib.sha256()
@@ -225,26 +226,29 @@
     changed = download(
         url,
         compressed_path,
         hash,
     )
 
     make_directory(dir_name)
-    if os.listdir(dir_name) == []:
+    marker_name = Path(compressed_path + ".unpacked")
+    if not marker_name.exists():
         from .debian import apt_install
 
         if compressed_path.endswith("tar.gz") or compressed_path.endswith(".tgz"):
             apt_install(["tar"])
             run_command("tar --directory=%s -zxvf %s" % (dir_name, compressed_path))
         elif compressed_path.endswith("zip"):
             apt_install(["unzip"])
             run_command("unzip %s -d %s" % (compressed_path, dir_name))
         else:
             raise Exception(compressed_path)
 
+        marker_name.open("w").write("")
+
         changed = True
 
     return {"changed": changed, "dir_name": dir_name}
 
 
 def last_modified(fname):
     try:
```

### Comparing `paracrine-0.0.5/paracrine/login.py` & `paracrine-0.0.6/paracrine/login.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/network.py` & `paracrine-0.0.6/paracrine/network.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/runner.py` & `paracrine-0.0.6/paracrine/runner.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/services/cockroachdb.py` & `paracrine-0.0.6/paracrine/services/cockroachdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,22 @@
 options = {}
 
 
 def dependencies():
     return [ntp, wireguard]
 
 
-cockroach_url = "https://binaries.cockroachdb.com/cockroach-v22.2.9.linux-amd64.tgz"
-cockroach_hash = "7ed169bf5f1f27bd49ab4e04a00068f7b44cff8a0672778b0f67d87ece3de07b"
-binary_path = "cockroach-v22.2.9.linux-amd64/cockroach"
+cockroach_version = "23.1.1"
+cockroach_url = (
+    f"https://binaries.cockroachdb.com/cockroach-v{cockroach_version}.linux-amd64.tgz"
+)
+cockroach_hash = "8197562ce59d1ac4f53f67c9d277827d382db13c5e650980942bcb5e5104bb4e"
+binary_path = f"cockroach-v{cockroach_version}.linux-amd64/cockroach"
+# FIXME
+cockroach_binary = f"/opt/cockroach-v{cockroach_version}.linux-amd64/{binary_path}"
 HOME_DIR = Path("/var/lib/cockroach")
 CERTS_DIR = HOME_DIR.joinpath("certs")
 USER = "cockroach"
 
 
 def bootstrap_local():
     store_path = Path(data_path()).joinpath("cockroach")
@@ -41,74 +46,79 @@
         compressed_root=data_path(),
     )
     cockroach = store_path.joinpath(binary_path)
     certs_dir = Path(config_path()).joinpath("cockroach-certs")
     make_directory(certs_dir)
     build_with_command(
         store_path.joinpath("ca.key"),
-        f"{cockroach} cert create-ca --certs-dir={certs_dir} --ca-key={store_path}/ca.key",
+        f"{cockroach} cert create-ca --certs-dir={certs_dir} --ca-key={store_path}/ca.key --overwrite --allow-ca-key-reuse",
     )
     build_with_command(
         certs_dir.joinpath("client.root.key"),
-        f"{cockroach} cert create-client root --certs-dir={certs_dir} --ca-key={store_path}/ca.key",
+        f"{cockroach} cert create-client root --certs-dir={certs_dir} --ca-key={store_path}/ca.key --overwrite",
+        deps=[f"{store_path}/ca.key"],
     )
 
     for ip in wireguard_ips().values():
         crt_path = certs_dir.joinpath(f"{ip}.crt")
         build_with_command(
             crt_path,
-            f"{cockroach} cert create-node localhost {ip} --certs-dir={certs_dir} --ca-key={store_path}/ca.key && mv {certs_dir.joinpath('node.crt')} {crt_path} && mv {certs_dir.joinpath('node.key')} {crt_path.with_suffix('.key')}",
+            f"{cockroach} cert create-node localhost {ip} --certs-dir={certs_dir} --ca-key={store_path}/ca.key --overwrite && mv {certs_dir.joinpath('node.crt')} {crt_path} && mv {certs_dir.joinpath('node.key')} {crt_path.with_suffix('.key')}",
+            deps=[f"{store_path}/ca.key"],
         )
 
 
-# FIXME
-cockroach_binary = (
-    "/opt/cockroach-v22.2.9.linux-amd64/cockroach-v22.2.9.linux-amd64/cockroach"
-)
-
-
 def core_run():
     unpacked = download_and_unpack(
         cockroach_url,
         cockroach_hash,
     )
     cockroach_path = Path(unpacked["dir_name"]).joinpath(binary_path)
     adduser(USER, HOME_DIR)
     make_directory(CERTS_DIR)
+    file_changes = False
     for fname in get_config_keys():
         if "cockroach-certs" not in fname:
             continue
         new_fname = CERTS_DIR.joinpath(
             fname.replace("configs/cockroach-certs/", "")
         ).as_posix()
         if wireguard_ip() in fname:
             new_fname = new_fname.replace(wireguard_ip(), "node")
-        set_file_contents(new_fname, get_config_file(fname), owner="cockroach")
-        set_mode(new_fname, "700")
+        file_changes = (
+            set_file_contents(new_fname, get_config_file(fname), owner="cockroach")
+            or file_changes
+        )
+        file_changes = set_mode(new_fname, "700") or file_changes
 
     COCKROACH_PORT = options.get("COCKROACH_PORT", 26257)
     SQL_PORT = options.get("SQL_PORT", 26258)
-    changes = set_file_contents_from_template(
+    service_file_changes = set_file_contents_from_template(
         "/etc/systemd/system/cockroach.service",
         "cockroach.service.j2",
         COCKROACH_PATH=cockroach_path,
         HOME_DIR=HOME_DIR,
         USER=USER,
         CERTS_DIR=CERTS_DIR,
         WIREGUARD_IP=wireguard_ip(),
         HTTP_PORT=options.get("HTTP_PORT", 8080),
         COCKROACH_PORT=COCKROACH_PORT,
         SQL_PORT=SQL_PORT,
         HOST_LIST=",".join(
             [f"{ip}:{COCKROACH_PORT}" for ip in wireguard_ips().values()]
         ),
     )
-    if changes:
+    if service_file_changes:
         systemctl_daemon_reload()
-    systemd_set("cockroach", enabled=True, running=True, restart=changes)
+    systemd_set(
+        "cockroach",
+        enabled=True,
+        running=True,
+        restart=file_changes or service_file_changes,
+    )
 
     if use_this_host("cockroach"):
         run_with_marker(
             HOME_DIR.joinpath("init_done"),
             f"{cockroach_binary} init --certs-dir={CERTS_DIR} --host={wireguard_ip()}:{COCKROACH_PORT}",
         )
```

### Comparing `paracrine-0.0.5/paracrine/services/pleroma.py` & `paracrine-0.0.6/paracrine/services/pleroma.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/services/postgresql.py` & `paracrine-0.0.6/paracrine/services/postgresql.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/services/wireguard.py` & `paracrine-0.0.6/paracrine/services/wireguard.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/systemd.py` & `paracrine-0.0.6/paracrine/systemd.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/templates/config.exs.j2` & `paracrine-0.0.6/paracrine/templates/config.exs.j2`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/templates/pleroma.nginx.j2` & `paracrine-0.0.6/paracrine/templates/pleroma.nginx.j2`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine/users.py` & `paracrine-0.0.6/paracrine/users.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/paracrine.egg-info/PKG-INFO` & `paracrine-0.0.6/paracrine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracrine
-Version: 0.0.5
+Version: 0.0.6
 Summary: A system deployment tool
 Author-email: Tom Parker-Shemilt <palfrey@tevp.net>
 Project-URL: Homepage, https://github.com/palfrey/paracrine
 Project-URL: Bug Tracker, https://github.com/palfrey/paracrine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `paracrine-0.0.5/paracrine.egg-info/SOURCES.txt` & `paracrine-0.0.6/paracrine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.5/pyproject.toml` & `paracrine-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "paracrine"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Tom Parker-Shemilt", email="palfrey@tevp.net" },
 ]
 description = "A system deployment tool"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `paracrine-0.0.5/tests/test_ssh.py` & `paracrine-0.0.6/tests/test_ssh.py`

 * *Files identical despite different names*

