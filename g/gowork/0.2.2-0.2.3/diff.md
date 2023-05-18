# Comparing `tmp/gowork-0.2.2.tar.gz` & `tmp/gowork-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gowork-0.2.2.tar", last modified: Thu Jul 21 21:08:16 2022, max compression
+gzip compressed data, was "gowork-0.2.3.tar", last modified: Thu May 18 17:00:29 2023, max compression
```

## Comparing `gowork-0.2.2.tar` & `gowork-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 21:08:16.177717 gowork-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-07-21 21:08:16.177717 gowork-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-07-21 21:08:07.000000 gowork-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 21:08:16.177717 gowork-0.2.2/gowork/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-07-21 21:08:07.000000 gowork-0.2.2/gowork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4056 2022-07-21 21:08:07.000000 gowork-0.2.2/gowork/databases.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-07-21 21:08:07.000000 gowork-0.2.2/gowork/handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-07-21 21:08:07.000000 gowork-0.2.2/gowork/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 21:08:16.177717 gowork-0.2.2/gowork/safe/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-07-21 21:08:07.000000 gowork-0.2.2/gowork/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-07-21 21:08:07.000000 gowork-0.2.2/gowork/safe/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 21:08:16.177717 gowork-0.2.2/gowork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-07-21 21:08:16.000000 gowork-0.2.2/gowork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-07-21 21:08:16.000000 gowork-0.2.2/gowork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 21:08:16.000000 gowork-0.2.2/gowork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-21 21:08:16.000000 gowork-0.2.2/gowork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-21 21:08:16.000000 gowork-0.2.2/gowork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-21 21:08:16.177717 gowork-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-07-21 21:08:07.000000 gowork-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:00:29.822595 gowork-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 17:00:29.822595 gowork-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-18 17:00:18.000000 gowork-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:00:29.822595 gowork-0.2.3/gowork/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:00:29.822595 gowork-0.2.3/gowork/safe/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/safe/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:00:29.822595 gowork-0.2.3/gowork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 17:00:29.000000 gowork-0.2.3/gowork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-18 17:00:29.000000 gowork-0.2.3/gowork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:00:29.000000 gowork-0.2.3/gowork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 17:00:29.000000 gowork-0.2.3/gowork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 17:00:29.000000 gowork-0.2.3/gowork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:00:29.822595 gowork-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-18 17:00:18.000000 gowork-0.2.3/setup.py
```

### Comparing `gowork-0.2.2/README.rst` & `gowork-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `gowork-0.2.2/gowork/databases.py` & `gowork-0.2.3/gowork/databases.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pyathena import connect
 from pyathena.pandas.util import as_pandas
 from sqlalchemy import create_engine
 import pandas as pd
 import glob
 import pathlib
 import base64
-
+import platform
 
 class AthenaGo:
     def __init__(self, name_connection: str):
         self.__decode(name_connection)
         self.__con = connect(aws_access_key_id=self.__cred['aws_access_key_id'],
                              aws_secret_access_key=self.__cred['aws_secret_access_key'],
                              s3_staging_dir=self.__cred['s3_staging_dir'],
@@ -79,14 +79,15 @@
     """This object load sql files and insert them into a dictionary to access via their key,
         which receives the same name as the file
     """
     def __init__(self, path: str):
         """
         :param path: Where your sql files are located
         """
+        self.__platform = '\\' if platform.system().__str__() == 'Windows' else '/'
         self.__queries = {}
         self.path = path
         self.__root = pathlib.Path().resolve().__str__()
         self.__loadfiles()
 
     def use(self, query_name: str):
         """Select which query do you want use
@@ -101,18 +102,18 @@
         return query.replace('%%','%').replace('%','%%')
 
     def __loadfiles(self):
         """
         Internal method that go through all files in directory and insert into a dictionary
         :return: None
         """
-        for path in glob.glob(f"{self.__root + '/' + self.path}/*.sql"):
-            self.__cachefile(path.split('/')[-1])
+        for path in glob.glob(f"{self.__root + self.__platform + self.path + self.__platform}*.sql"):
+            self.__cachefile(path.split(self.__platform)[-1])
 
     def __cachefile(self, file: str):
         """
         Insert into dictionary
         :param file: File name
         :return: None
         """
-        with open(self.__root + '/' + self.path + '/' + file, 'r', encoding='utf-8') as line:
+        with open(self.__root + self.__platform + self.path + self.__platform + file, 'r', encoding='utf-8') as line:
             self.__queries[file.replace('.sql', '')] = self.__percsign(line.read())
```

### Comparing `gowork-0.2.2/gowork/handler.py` & `gowork-0.2.3/gowork/handler.py`

 * *Files identical despite different names*

### Comparing `gowork-0.2.2/gowork/monitor.py` & `gowork-0.2.3/gowork/monitor.py`

 * *Files identical despite different names*

### Comparing `gowork-0.2.2/gowork/safe/configs.py` & `gowork-0.2.3/gowork/safe/configs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import gowork
 import json
 import os
 import base64
-
+import platform
 
 class Credentials:
     def __init__(self):
-        self.__root = '/'.join(gowork.__file__.split('/')[:-1] + ['safe', 'secret_keys.json'])
+        self.__platform = '\\' if platform.system().__str__() == 'Windows' else '/'
+        self.__root = self.__platform.join(gowork.__file__.split(self.__platform)[:-1] + ['safe', 'secret_keys.json'])
         self.__creds = {}
 
     def insert(self, name: str, connector: str, credentials: dict, encode=[]):
         name = name.lower()
         connector = connector.lower()
 
         self.__load()
@@ -39,7 +40,9 @@
             with open(self.__root, 'r', encoding='utf-8') as file:
                 self.__creds = json.load(file)
 
     def __encode(self, credentials: dict, keys: list):
         for key in keys:
             credentials[key] = {'encode': base64.b64encode(credentials[key].encode('utf-8')).decode('utf-8')}
         return credentials
+
+
```

### Comparing `gowork-0.2.2/setup.py` & `gowork-0.2.3/setup.py`

 * *Files identical despite different names*

