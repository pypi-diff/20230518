# Comparing `tmp/scandal-0.1.5.tar.gz` & `tmp/scandal-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scandal-0.1.5.tar", max compression
+gzip compressed data, was "scandal-0.1.6.tar", max compression
```

## Comparing `scandal-0.1.5.tar` & `scandal-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       10 2023-05-11 17:44:44.660535 scandal-0.1.5/README.md
--rw-r--r--   0        0        0      693 2023-05-11 17:44:44.660535 scandal-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2467 2023-05-11 17:44:44.660535 scandal-0.1.5/scandal/__init__.py
--rw-r--r--   0        0        0      168 2023-05-11 17:44:44.660535 scandal-0.1.5/scandal/__main__.py
--rw-r--r--   0        0        0     3056 2023-05-11 17:44:44.660535 scandal-0.1.5/scandal/_auth.py
--rw-r--r--   0        0        0      114 2023-05-11 17:44:44.660535 scandal-0.1.5/scandal/_connection.py
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 scandal-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-05-18 09:11:52.614426 scandal-0.1.6/README.md
+-rw-r--r--   0        0        0      693 2023-05-18 09:11:52.614426 scandal-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2467 2023-05-18 09:11:52.614426 scandal-0.1.6/scandal/__init__.py
+-rw-r--r--   0        0        0      522 2023-05-18 09:11:52.614426 scandal-0.1.6/scandal/__main__.py
+-rw-r--r--   0        0        0     3355 2023-05-18 09:11:52.614426 scandal-0.1.6/scandal/_auth.py
+-rw-r--r--   0        0        0      114 2023-05-18 09:11:52.614426 scandal-0.1.6/scandal/_connection.py
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 scandal-0.1.6/PKG-INFO
```

### Comparing `scandal-0.1.5/pyproject.toml` & `scandal-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scandal-0.1.5/scandal/__init__.py` & `scandal-0.1.6/scandal/__init__.py`

 * *Files identical despite different names*

### Comparing `scandal-0.1.5/scandal/_auth.py` & `scandal-0.1.6/scandal/_auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+import json
+import os.path
 import time
 import webbrowser
 
 import jwt
 import keyring
 import requests
 
-SERVICE = "scandal"
+SERVICE = "scandal-py"
 AUTH_DOMAIN = "http://localhost:3000"
 CLIENT_ID = "app_3JQW6ThZHnj2VJMlemk6D"
 GRANT_TYPE = "urn:ietf:params:oauth:grant-type:device_code"
+
 # Refresh token 5 minutes before it expires
 EXPIRY_WINDOW = 5 * 60
 
+# Check for local development
+creds_file = os.path.join(os.path.dirname(__file__), "../../crowbar/.oauth.creds.json")
+if os.path.exists(creds_file):
+    with open(creds_file) as f:
+        creds = json.load(f)
+        CLIENT_ID = creds["clientCreds"][SERVICE]["clientId"]
+
 
 def auth_user():
     # _try_delete_password(SERVICE, "access_token")
     # _try_delete_password(SERVICE, "refresh_token")
 
     access_token = keyring.get_password(SERVICE, "access_token")
     refresh_token = keyring.get_password(SERVICE, "refresh_token")
@@ -45,15 +55,15 @@
 
     resp = requests.post(
         f"{AUTH_DOMAIN}/oauth/device",
         data={
             "client_id": CLIENT_ID,
             # TODO(ngates): should this be scandal instead?
             "audience": "https://scandal.fulcrum.so",
-            "scope": "read offline_access",
+            "scope": "offline_access",
         },
     )
     if not resp.ok:
         raise Exception(f"{resp.status_code}: {resp.text}")
     code_resp = resp.json()
 
     expiry = time.time() + code_resp["expires_in"]
```

### Comparing `scandal-0.1.5/PKG-INFO` & `scandal-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scandal
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Nicholas Gates
 Author-email: nick@nickgates.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

