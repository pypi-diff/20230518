# Comparing `tmp/habu-python-api-2.0.2.tar.gz` & `tmp/habu-python-api-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/roopakgupta/habu/habu-api/dist/.tmp-hcdkvtns/habu-python-api-2.0.2.tar", last modified: Thu Apr 20 03:56:18 2023, max compression
+gzip compressed data, was "/Users/roopakgupta/habu/habu-api/dist/.tmp-opy_cghn/habu-python-api-2.0.3.tar", last modified: Thu May 18 15:07:42 2023, max compression
```

## Comparing `habu-python-api-2.0.2.tar` & `habu-python-api-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-04-20 03:56:18.929182 habu-python-api-2.0.2/
--rw-r--r--   0 roopakgupta   (501) staff       (20)      880 2023-04-20 03:56:18.928636 habu-python-api-2.0.2/PKG-INFO
--rw-r--r--   0 roopakgupta   (501) staff       (20)      463 2023-02-23 23:56:27.000000 habu-python-api-2.0.2/README.md
--rw-r--r--   0 roopakgupta   (501) staff       (20)      133 2021-09-13 19:52:09.000000 habu-python-api-2.0.2/pyproject.toml
--rw-r--r--   0 roopakgupta   (501) staff       (20)       38 2023-04-20 03:56:18.929333 habu-python-api-2.0.2/setup.cfg
--rw-r--r--   0 roopakgupta   (501) staff       (20)      739 2023-04-20 03:55:36.000000 habu-python-api-2.0.2/setup.py
-drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-04-20 03:56:18.920796 habu-python-api-2.0.2/src/
-drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-04-20 03:56:18.924456 habu-python-api-2.0.2/src/habu_api/
--rw-r--r--   0 roopakgupta   (501) staff       (20)        0 2021-09-13 19:52:09.000000 habu-python-api-2.0.2/src/habu_api/__init__.py
--rw-r--r--   0 roopakgupta   (501) staff       (20)     3606 2023-04-20 03:55:36.000000 habu-python-api-2.0.2/src/habu_api/cleanRoom.py
-drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-04-20 03:56:18.927894 habu-python-api-2.0.2/src/habu_python_api.egg-info/
--rw-r--r--   0 roopakgupta   (501) staff       (20)      880 2023-04-20 03:56:18.000000 habu-python-api-2.0.2/src/habu_python_api.egg-info/PKG-INFO
--rw-r--r--   0 roopakgupta   (501) staff       (20)      256 2023-04-20 03:56:18.000000 habu-python-api-2.0.2/src/habu_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 roopakgupta   (501) staff       (20)        1 2023-04-20 03:56:18.000000 habu-python-api-2.0.2/src/habu_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 roopakgupta   (501) staff       (20)        9 2023-04-20 03:56:18.000000 habu-python-api-2.0.2/src/habu_python_api.egg-info/top_level.txt
+drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-05-18 15:07:42.624499 habu-python-api-2.0.3/
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      880 2023-05-18 15:07:42.623831 habu-python-api-2.0.3/PKG-INFO
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      463 2023-02-23 23:56:27.000000 habu-python-api-2.0.3/README.md
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      133 2021-09-13 19:52:09.000000 habu-python-api-2.0.3/pyproject.toml
+-rw-r--r--   0 roopakgupta   (501) staff       (20)       38 2023-05-18 15:07:42.624708 habu-python-api-2.0.3/setup.cfg
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      739 2023-05-18 15:06:42.000000 habu-python-api-2.0.3/setup.py
+drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-05-18 15:07:42.614878 habu-python-api-2.0.3/src/
+drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-05-18 15:07:42.618723 habu-python-api-2.0.3/src/habu_api/
+-rw-r--r--   0 roopakgupta   (501) staff       (20)        0 2021-09-13 19:52:09.000000 habu-python-api-2.0.3/src/habu_api/__init__.py
+-rw-r--r--   0 roopakgupta   (501) staff       (20)     3809 2023-05-18 15:06:42.000000 habu-python-api-2.0.3/src/habu_api/cleanRoom.py
+drwxr-xr-x   0 roopakgupta   (501) staff       (20)        0 2023-05-18 15:07:42.622982 habu-python-api-2.0.3/src/habu_python_api.egg-info/
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      880 2023-05-18 15:07:42.000000 habu-python-api-2.0.3/src/habu_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 roopakgupta   (501) staff       (20)      256 2023-05-18 15:07:42.000000 habu-python-api-2.0.3/src/habu_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 roopakgupta   (501) staff       (20)        1 2023-05-18 15:07:42.000000 habu-python-api-2.0.3/src/habu_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 roopakgupta   (501) staff       (20)        9 2023-05-18 15:07:42.000000 habu-python-api-2.0.3/src/habu_python_api.egg-info/top_level.txt
```

### Comparing `habu-python-api-2.0.2/PKG-INFO` & `habu-python-api-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habu-python-api
-Version: 2.0.2
+Version: 2.0.3
 Summary: Habu Python API
 Home-page: https://github.com/deklareddotcom/habu-api
 Author: Habu
 Author-email: support@habu.com
 Project-URL: Bug Tracker, https://github.com/deklareddotcom/habu-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `habu-python-api-2.0.2/setup.py` & `habu-python-api-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="habu-python-api",
-    version="2.0.2",
+    version="2.0.3",
     author="Habu",
     author_email="support@habu.com",
     description="Habu Python API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deklareddotcom/habu-api",
     project_urls={
```

### Comparing `habu-python-api-2.0.2/src/habu_api/cleanRoom.py` & `habu-python-api-2.0.3/src/habu_api/cleanRoom.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import datetime
-import json
 import os
 import pytz
 
 import requests, base64
 
-from requests.auth import HTTPBasicAuth
 from urllib3.exceptions import InsecureRequestWarning
 
 class BaseApi():
     def __init__(self):
         requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
         self.api = os.getenv("HABU_API", "https://localhost:9443")
         self.access_token, self.expire_time = self.login()
@@ -17,15 +15,15 @@
     def login(self):
         client = os.getenv("HABU_API_CLIENT")
         secret = os.getenv("HABU_API_SECRET")
 
         if not client or not secret:
             raise Exception("API Client and Secret must be defined in your environment. Please check documentation!")
 
-        usrPass = "%s:%s" %(client, secret)
+        usrPass = "%s:%s" % (client, secret)
         b64Val = base64.b64encode(usrPass.encode()).decode()
 
         data = {'grant_type': 'client_credentials'}
         response = requests.post("%s/v1/oauth/token" % self.api,
                                  headers={"Authorization": "Basic %s" % b64Val},
                                  data=data,
                                  verify=False)
@@ -39,46 +37,48 @@
         return data["accessToken"], datetime.datetime.strptime(data["expiresAt"], '%Y-%m-%dT%H:%M:%S.%f%z')
 
     def get_token(self):
         if self.expire_time < pytz.UTC.localize(datetime.datetime.now()):
             self.access_token, self.expire_time = self.login()
         return self.access_token
 
-    def post(self, url, key=None):
+    def post(self, url, body=None):
         response = requests.post(url,
                                  verify=False,
-                                 headers={'Authorization': 'Bearer %s' %self.get_token()})
+                                 headers={'Authorization': 'Bearer %s' % self.get_token()},
+                                 json=body)
         if response.status_code != 200:
             response.raise_for_status()
-        return response.json()[key]
+        return response.json()
 
     def get(self, url, key=None):
         response = requests.get(url,
                                 verify=False,
-                                headers={"Authorization": "Bearer %s" %self.get_token()})
+                                headers={"Authorization": "Bearer %s" % self.get_token()})
         if response.status_code != 200:
             response.raise_for_status()
 
         if len(response.text) == 0:
             return []
         else:
             if key:
                 return response.json()[key]
             else:
                 return response.json()
 
+
 class CleanRoom(BaseApi):
     def __init__(self):
         BaseApi.__init__(self)
         self.org_uuid = os.getenv("HABU_ORGANIZATION")
         if not self.org_uuid:
             raise Exception("Organization must be defined in your environment. Please check documentation!")
 
     def get_clean_rooms(self):
-        return self.get("%s/v1/cleanrooms" %self.api)
+        return self.get("%s/v1/cleanrooms" % self.api)
 
     def get_clean_room_questions(self, cleanroom_uuid):
         return self.get("%s/v1/cleanrooms/%s/cleanroom-questions"
                         % (self.api, cleanroom_uuid))
 
     def get_question_runs(self, question_uuid, limit=500, offset=0):
         return self.get("%s/v1/cleanroom-questions/%s/cleanroom-question-runs?limit=%s&offset=%s"
@@ -86,8 +86,12 @@
 
     def get_question_run_data(self, run_uuid, limit=500, offset=0):
         return self.get("%s/v1/cleanroom-question-runs/%s/data?limit=%s&offset=%s"
                         % (self.api, run_uuid, limit, offset))
 
     def get_run_data_count(self, run_uuid):
         return self.get("%s/v1/cleanroom-question-runs/%s/data/count"
-                        % (self.api, run_uuid))
+                        % (self.api, run_uuid))
+
+    def create_run(self, question_uuid, create_run_parameters):
+        return self.post("%s/v1/cleanroom-questions/%s/create-run"
+                         % (self.api, question_uuid), create_run_parameters)
```

### Comparing `habu-python-api-2.0.2/src/habu_python_api.egg-info/PKG-INFO` & `habu-python-api-2.0.3/src/habu_python_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habu-python-api
-Version: 2.0.2
+Version: 2.0.3
 Summary: Habu Python API
 Home-page: https://github.com/deklareddotcom/habu-api
 Author: Habu
 Author-email: support@habu.com
 Project-URL: Bug Tracker, https://github.com/deklareddotcom/habu-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

