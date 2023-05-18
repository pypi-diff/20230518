# Comparing `tmp/umapi-client-2.9.tar.gz` & `tmp/umapi_client-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/umapi-client-2.9.tar", last modified: Wed Nov 15 01:47:38 2017, max compression
+gzip compressed data, was "umapi_client-3.0.tar", max compression
```

## Comparing `umapi-client-2.9.tar` & `umapi_client-3.0.tar`

### file list

```diff
@@ -1,21 +1,12 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-11-15 01:47:38.000000 umapi-client-2.9/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client/
--rw-r--r--   0 travis    (2000) travis    (2000)     1553 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)    10469 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/api.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3803 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/auth.py
--rw-r--r--   0 travis    (2000) travis    (2000)    23658 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/connection.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2589 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/error.py
--rw-r--r--   0 travis    (2000) travis    (2000)    22815 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/functional.py
--rw-r--r--   0 travis    (2000) travis    (2000)    10696 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/legacy.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1154 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/version.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     1152 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      431 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/not-zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)       46 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       13 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)     1811 2017-11-15 01:45:32.000000 umapi-client-2.9/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)       92 2017-11-15 01:47:38.000000 umapi-client-2.9/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     2964 2017-11-15 01:45:32.000000 umapi-client-2.9/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1152 2017-11-15 01:47:38.000000 umapi-client-2.9/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-05-18 20:14:47.088379 umapi_client-3.0/LICENSE
+-rw-r--r--   0        0        0     2082 2023-05-18 20:14:47.088379 umapi_client-3.0/README.md
+-rw-r--r--   0        0        0     1226 2023-05-18 20:14:47.088379 umapi_client-3.0/pyproject.toml
+-rw-r--r--   0        0        0     1543 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/__init__.py
+-rw-r--r--   0        0        0    12272 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/api.py
+-rw-r--r--   0        0        0     4971 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/auth.py
+-rw-r--r--   0        0        0    24495 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/connection.py
+-rw-r--r--   0        0        0     2606 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/error.py
+-rw-r--r--   0        0        0    14377 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/functional.py
+-rw-r--r--   0        0        0     1137 2023-05-18 20:14:47.088379 umapi_client-3.0/umapi_client/version.py
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 umapi_client-3.0/setup.py
+-rw-r--r--   0        0        0     3502 1970-01-01 00:00:00.000000 umapi_client-3.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `umapi-client-2.9/umapi_client/__init__.py` & `umapi_client-3.0/umapi_client/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2017 Adobe Systems Incorporated.  All rights reserved.
+# Copyright (c) 2016-2021 Adobe Inc.  All rights reserved.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -15,13 +15,14 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .api import Action, QuerySingle, QueryMultiple
+from .auth import JWTAuth, OAuthS2S
 from .connection import Connection
 from .error import BatchError, ClientError, RequestError, ServerError, UnavailableError, ArgumentError
-from .functional import IdentityTypes, GroupTypes, RoleTypes, IfAlreadyExistsOptions
+from .functional import IdentityType, IfAlreadyExistsOption
 from .functional import UserAction, UserQuery, UsersQuery
-from .functional import UserGroupAction, GroupsQuery
+from .functional import GroupAction, GroupsQuery
 from .version import __version__
```

### Comparing `umapi-client-2.9/umapi_client/api.py` & `umapi_client-3.0/umapi_client/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2017 Adobe Systems Incorporated.  All rights reserved.
+# Copyright (c) 2016-2021 Adobe Inc.  All rights reserved.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -14,16 +14,14 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import six
-
 from .connection import Connection
 
 
 class Action:
     """
     An sequence of commands for the API to perform on a single object.
     """
@@ -72,15 +70,15 @@
         the order in which the args were specified.  Thus, if you care about specific ordering,
         you must make multiple calls to append in that order.  Luckily, append returns
         the Action so you can compose easily: Action(...).append(...).append(...).
         See also insert, below.
         :param kwargs: the key/value pairs to add
         :return: the action
         """
-        for k, v in six.iteritems(kwargs):
+        for k, v in kwargs.items():
             self.commands.append({k: v})
         return self
 
     def insert(self, **kwargs):
         """
         Insert commands at the beginning of the sequence.
 
@@ -91,15 +89,15 @@
 
         Also, since the order of iterated kwargs is not guaranteed (in Python 2.x),
         you should really only call insert with one keyword at a time.  See the doc of append
         for more details.
         :param kwargs: the key/value pair to append first
         :return: the action, so you can append Action(...).insert(...).append(...)
         """
-        for k, v in six.iteritems(kwargs):
+        for k, v in kwargs.items():
             self.commands.insert(0, {k: v})
         return self
 
     def report_command_error(self, error_dict):
         """
         Report a server error executing a command.
 
@@ -123,14 +121,47 @@
         """
         if self.split_actions:
             # throttling split this action, get errors from the split
             return [dict(e) for s in self.split_actions for e in s.errors]
         else:
             return [dict(e) for e in self.errors]
 
+    def maybe_split_groups(self, max_groups):
+        """
+        Check if group lists in add/remove directives should be split and split them if needed
+        :param max_groups: Max group list size
+        :return: True if at least one command was split, False if none were split
+        """
+        split_commands = []
+        # return True if we split at least once
+        maybe_split = False
+        valid_step_keys = ['add', 'remove']
+        for command in self.commands:
+            # commands are assumed to contain a single key
+            step_key, step_args = next(iter(command.items()))
+            if step_key not in valid_step_keys or not isinstance(step_args, dict):
+                split_commands.append(command)
+                continue
+            new_commands = [command]
+            while True:
+                new_command = {step_key: {}}
+                for group_type, groups in command[step_key].items():
+                    if len(groups) > max_groups:
+                        command[step_key][group_type], new_command[step_key][group_type] = \
+                            groups[0:max_groups], groups[max_groups:]
+                if new_command[step_key]:
+                    new_commands.append(new_command)
+                    command = new_command
+                    maybe_split = True
+                else:
+                    break
+            split_commands += new_commands
+        self.commands = split_commands
+        return maybe_split
+
 
 class QueryMultiple:
     """
     A QueryMultiple runs a query against a connection.  The results can be iterated or fetched in bulk.
     """
     def __init__(self, connection, object_type, url_params=None, query_params=None):
         # type: (Connection, str, list, dict) -> None
@@ -145,35 +176,43 @@
         self.conn = connection
         self.object_type = object_type
         self.url_params = url_params if url_params else []
         self.query_params = query_params if query_params else {}
         self._results = []
         self._next_item_index = 0
         self._next_page_index = 0
+        self._total_count = 0
+        self._page_size = 1
+        self._page_count = 0
+        self._page_number = 1
         self._last_page_seen = False
 
     def reload(self):
         """
         Rerun the query (lazily).
         The results will contain any values on the server side that have changed since the last run.
         :return: None
         """
         self._results = []
         self._next_item_index = 0
         self._next_page_index = 0
+        self._total_count = 0
+        self._page_count = 0
+        self._page_size = 0
+        self._page_number = 1
         self._last_page_seen = False
 
     def _next_page(self):
         """
         Fetch the next page of the query.
         """
         if self._last_page_seen:
             raise StopIteration
-        new, self._last_page_seen = self.conn.query_multiple(self.object_type, self._next_page_index,
-                                                             self.url_params, self.query_params)
+        new, self._last_page_seen, self._total_count, self._page_count, self._page_number, self._page_size = \
+            self.conn.query_multiple(self.object_type, self._next_page_index, self.url_params, self.query_params)
         self._next_page_index += 1
         if len(new) == 0:
             self._last_page_seen = True  # don't bother with next page if nothing was returned
         else:
             self._results += new
 
     def _next_item(self):
@@ -213,14 +252,17 @@
         :return: a list of all the results.
         """
         while not self._last_page_seen:
             self._next_page()
         self._next_item_index = len(self._results)
         return list(self._results)
 
+    def stats(self):
+        return self._total_count, self._page_count, self._page_size, self._page_number
+
 
 class QuerySingle:
     """
     Look for a single object
     """
     def __init__(self, connection, object_type, url_params=None, query_params=None):
         # type: (Connection, str, list, dict) -> None
```

### Comparing `umapi-client-2.9/umapi_client/auth.py` & `umapi_client-3.0/umapi_client/auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2017 Adobe Systems Incorporated.  All rights reserved.
+# Copyright (c) 2016-2021 Adobe Inc.  All rights reserved.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,85 +17,116 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import datetime as dt
 import time
 
-import jwt  # package name is PyJWT in setup
+import jwt
 import requests
-import six.moves.urllib.parse as urlparse
+import urllib.parse as urlparse
+import logging
 
-
-class JWT(object):
-    def __init__(self, org_id, tech_acct, ims_host, api_key, key_file):
-        self.expiry_time = int(time.time()) + 60*60*24
-        self.org_id = org_id
-        self.tech_acct = tech_acct
-        self.ims_host = ims_host
-        self.api_key = api_key
-
-        self.key = key_file.read()
-        key_file.close()
-
-    def __call__(self):
-        payload = {
-            "exp": self.expiry_time,
-            "iss": self.org_id,
-            "sub": self.tech_acct,
-            "aud": "https://" + self.ims_host + "/c/" + self.api_key,
-            "https://" + self.ims_host + "/s/" + "ent_user_sdk": True
-        }
-
-        # create JSON Web Token
-        # noinspection PyUnresolvedReferences
-        jwt_token = jwt.encode(payload, self.key, algorithm='RS256')
-        # decode bytes into string
-        return jwt_token.decode("utf-8")
+logger = logging.getLogger(__name__)
 
 
-class AccessRequest(object):
-    def __init__(self, endpoint, api_key, client_secret, jwt_token):
-        self.endpoint = endpoint
-        self.api_key = api_key
+class AdobeAuthBase(requests.auth.AuthBase):
+    def __init__(self, client_id, client_secret, auth_host, auth_endpoint,
+                 ssl_verify):
+        self.client_id = client_id
         self.client_secret = client_secret
-        self.jwt_token = jwt_token
+        self.auth_host = auth_host
+        self.auth_endpoint = auth_endpoint
+        self.ssl_verify = ssl_verify
         self.expiry = None
+        self.token = None
 
-    def __call__(self):
+    def set_expiry(self, expires_in):
+        expires_in = int(round(expires_in/1000))
+        self.expiry = dt.datetime.now() + dt.timedelta(seconds=expires_in)
+
+    def __call__(self, r):
+        if self.token is None or self.expiry is None or \
+           self.expiry <= dt.datetime.now():
+            self.refresh_token()
+        r.headers['Content-type'] = 'application/json'
+        r.headers['Accept'] = 'application/json'
+        r.headers['x-api-key'] = self.client_id
+        r.headers['Authorization'] = 'Bearer ' + self.token
+        return r
+    
+    def refresh_token(self):
+        logger.info("auth token is missing or expired - refreshing now")
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Cache-Control": "no-cache",
         }
-        body = urlparse.urlencode({
-            "client_id": self.api_key,
-            "client_secret": self.client_secret,
-            "jwt_token": self.jwt_token
-        })
 
-        r = requests.post(self.endpoint, headers=headers, data=body)
+        endpoint = f"https://{self.auth_host}/{self.auth_endpoint.strip('/')}/"
+
+        r = requests.post(endpoint, headers=headers, data=self.post_body(),
+                          verify=self.ssl_verify)
+
         if r.status_code != 200:
-            raise RuntimeError("Unable to authorize against {}:\n"
-                               "Response Code: {:d}, Response Text: {}\n"
-                               "Response Headers: {}]".format(self.endpoint, r.status_code, r.text, r.headers))
+            raise RuntimeError(f"Unable to authorize against {endpoint}:\n"
+                               f"Response Code: {r.status_code}, Response Text: {r.text}\n"
+                               f"Response Headers: {r.headers}]")
 
         self.set_expiry(r.json()['expires_in'])
 
-        return r.json()['access_token']
+        logger.debug("token expiration: %s", self.expiry)
+
+        self.token = r.json()['access_token']
+
+
+class OAuthS2S(AdobeAuthBase):
+    def __init__(self, client_id, client_secret,
+                 auth_host='ims-na1.adobelogin.com',
+                 auth_endpoint='/ims/token/v2',
+                 ssl_verify=True):
+        logger.info("Auth type: OAuthS2S")
+        super().__init__(
+            client_id, client_secret, auth_host, auth_endpoint, ssl_verify
+        )
+
+    def post_body(self):
+        return urlparse.urlencode({
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
+            "grant_type": "client_credentials",
+            "scope": "openid,AdobeID,user_management_sdk",
+        })
 
     def set_expiry(self, expires_in):
-        expires_in = int(round(expires_in/1000))
         self.expiry = dt.datetime.now() + dt.timedelta(seconds=expires_in)
 
 
-# noinspection PyUnresolvedReferences
-class Auth(requests.auth.AuthBase):
-    def __init__(self, api_key, access_token):
-        self.api_key = api_key
-        self.access_token = access_token
+class JWTAuth(AdobeAuthBase):
+    def __init__(self, org_id, client_id, client_secret, tech_acct_id,
+                 priv_key_data, ssl_verify=True,
+                 auth_host='ims-na1.adobelogin.com',
+                 auth_endpoint='/ims/exchange/jwt/'):
+        logger.info("Auth type: JWTAuth")
+        self.org_id = org_id
+        self.tech_acct_id = tech_acct_id
+        self.priv_key_data = priv_key_data
+        super().__init__(
+            client_id, client_secret, auth_host, auth_endpoint, ssl_verify
+        )
 
-    def __call__(self, r):
-        r.headers['Content-type'] = 'application/json'
-        r.headers['Accept'] = 'application/json'
-        r.headers['x-api-key'] = self.api_key
-        r.headers['Authorization'] = 'Bearer ' + self.access_token
-        return r
+    def jwt_token(self):
+        payload = {
+            "exp": int(time.time()) + 60*60*24,
+            "iss": self.org_id,
+            "sub": self.tech_acct_id,
+            "aud": "https://" + self.auth_host + "/c/" + self.client_id,
+            "https://" + self.auth_host + "/s/" + "ent_user_sdk": True
+        }
+
+        return jwt.encode(payload, self.priv_key_data, algorithm='RS256')
+
+    def post_body(self):
+        return urlparse.urlencode({
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
+            "jwt_token": self.jwt_token()
+        })
```

### Comparing `umapi-client-2.9/umapi_client/connection.py` & `umapi_client-3.0/umapi_client/connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2017 Adobe Systems Incorporated.  All rights reserved.
+# Copyright (c) 2016-2021 Adobe Inc.  All rights reserved.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,138 +16,144 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import json
 import logging
+import os
 from email.utils import parsedate_tz, mktime_tz
 from platform import python_version, version as platform_version
 from random import randint
 from time import time, sleep, gmtime, strftime
-
+from uuid import uuid4
+from datetime import datetime
 import requests
-import six
-import six.moves.urllib.parse as urlparse
+import io
+import urllib.parse as urlparse
 
-from .auth import JWT, Auth, AccessRequest
+from .auth import JWTAuth
 from .error import BatchError, UnavailableError, ClientError, RequestError, ServerError, ArgumentError
 from .version import __version__ as umapi_version
 
 
+class APIResult:
+    success_codes = [200, 201, 204]
+    timeout_codes = [429, 502, 503, 504]
+    client_error = lambda self, x: 201 <= x < 200
+    request_error = lambda self, x: 400 <= x < 500
+
+    def __init__(self, result=None, success=False, timeout=None):
+        self.result = result
+        self.success = success
+        self.timeout = timeout
+        self.status_code = result.status_code if hasattr(result, 'status_code') else 'Error'
+
+    def check_result(self):
+        if self.result.status_code in self.success_codes:
+            self.success = True
+            return self
+        if self.result.status_code in self.timeout_codes:
+            self.success = False
+            self.timeout = self.get_timeout()
+            return self
+        if self.client_error(self.result.status_code):
+            raise ClientError("Unexpected HTTP Status {:d}: {}".format(self.result.status_code, self.result.text), self.result)
+        if self.request_error(self.result.status_code):
+            raise RequestError(self.result)
+        raise ServerError(self.result)
+
+    def get_timeout(self):
+        if "Retry-After" in self.result.headers:
+            advice = self.result.headers["Retry-After"]
+            advised_time = parsedate_tz(advice)
+            if advised_time is not None:
+                # header contains date
+                return int(mktime_tz(advised_time) - time())
+            else:
+                # header contains delta seconds
+                return int(advice)
+        return 0
+
 class Connection:
     """
-    An org-specific, authorized connection to the UMAPI service.  Each method
+    An org-specific, authenticated connection to the UMAPI service.  Each method
     makes a single call on the endpoint and returns the result (or raises an error).
     """
+    mock_env_var = "UMAPI_MOCK"
 
     def __init__(self,
                  org_id,
-                 auth_dict=None,
-                 auth=None,
-                 ims_host="ims-na1.adobelogin.com",
-                 ims_endpoint_jwt="/ims/exchange/jwt/",
-                 user_management_endpoint="https://usermanagement.adobe.io/v2/usermanagement",
+                 auth,
+                 endpoint="https://usermanagement.adobe.io/v2/usermanagement",
                  test_mode=False,
-                 logger=logging.getLogger("umapi_client"),
-                 retry_max_attempts=4,
-                 retry_first_delay=15,
-                 retry_random_delay=5,
-                 timeout_seconds=120.0,
-                 throttle_actions=10,
-                 throttle_commands=10,
-                 throttle_groups=10,
-                 user_agent=None,
-                 **kwargs):
+                 ssl_verify=True,
+                 timeout=120.0,
+                 max_retries=4,
+                 user_agent=None):
         """
         Open a connection for the given parameters that has the given options.
-        The connection is authorized and the auth token reused on all calls.
+        The connection is authenticated and the auth token reused on all calls.
 
-        Required parameters.  You must specify org_id and one of auth *or* auth_dict
+        Required parameters.
         :param org_id: string OrganizationID from Adobe.IO integration data
-        :param auth_dict: a dictionary with auth information (see below)
-        :param auth: a umapi_client.auth.Auth object containing authorization
-
-        Auth data: if you supply an auth_dict, it must have values for these keys:
-        :param tech_acct_id: string technical account ID from Adobe.IO integration data
-        :param api_key: string api_key from Adobe.IO integration data
-        :param client_secret: string client secret from Adobe.IO integration data
-        and one of:
-        :param private_key_file: path to local private key file that matches Adobe.IO public key for integration
-        or:
-        :param private_key_data: the contents of the private_key_file (PEM format)
-        (NOTE: for compatibility with User Sync config files, the key names priv_key_path and tech_acct
-         are accepted as aliases for private_key_file and tech_acct_id, respectively.)
+        :param auth: a umapi_client.auth object that handles authentication
 
         Optional connection parameters (defaults are for Adobe production):
-        :param ims_host: the IMS host which will exchange your JWT for an access token
-        :param ims_endpoint_jwt: the exchange token endpoint on the IMS host
-        :param user_management_endpoint: the User Management API service root endpoint
+        :param endpoint: the User Management API service root endpoint
 
         Behavioral options for the connection:
         :param test_mode: Whether to pass the server-side "test mode" flag when executing actions
-        :param logger: The log handler to use (None suppresses logging, default is named "umapi_client")
-        :param retry_max_attempts: How many times to retry on temporary errors
-        :param retry_first_delay: The time to delay first retry (grows exponentially from there)
-        :param retry_random_delay: The max random delay to add on each exponential backoff retry
-        :param timeout_seconds: How many seconds to wait for server response (<= 0 or None means forever)
-        :param throttle_actions: Max number of actions to pack into a single call
-        :param throttle_commands: Max number of commands allowed in a single action
-        :param throttle_groups: Max number of groups to add/remove to/from a user
-        :param user_agent: (optional) string to use as User-Agent header (umapi-client/version data will be added)
-
-        Additional keywords are allowed to make it easy to pass a big dictionary with other values
-        :param kwargs: any keywords passed that we ignore.
+        :param timeout: How many seconds to wait for server response (<= 0 or None means forever)
+        :param ssl_verify:
         """
+        self.logger = logging.getLogger(__name__)
+        # for testing we mock the server, either by using an http relay
+        # which relays and records the requests and responses, or by
+        # using a robot which plays back a previously recorded run.
+        mock_spec = os.getenv(self.mock_env_var, None)
+        if mock_spec:
+            if mock_spec not in ["proxy", "playback"]:
+                raise ArgumentError("Unknown value for %s: %s" % (self.mock_env_var, mock_spec))
+            self.logger.warning("%s override specified as '%s'", self.mock_env_var, mock_spec)
+            # mocked servers don't support https
+            if endpoint.lower().startswith("https://"):
+                endpoint = "http" + endpoint[5:]
+            # playback servers don't use authentication
+            if mock_spec == "playback":
+                auth = JWTAuth("mock", "mock", "mock", "mock", "mock")
+
         self.org_id = str(org_id)
-        self.endpoint = user_management_endpoint
+        self.auth = auth
+        self.endpoint = endpoint
         self.test_mode = test_mode
-        self.logger = logger
-        self.retry_max_attempts = retry_max_attempts
-        self.retry_first_delay = retry_first_delay
-        self.retry_random_delay = retry_random_delay
-        self.timeout = float(timeout_seconds) if timeout_seconds and float(timeout_seconds) > 0.0 else None
-        self.throttle_actions = max(int(throttle_actions), 1)
-        self.throttle_commands = max(int(throttle_commands), 1)
-        self.throttle_groups = max(int(throttle_groups), 1)
+        self.retry_max_attempts = max_retries
+        self.retry_first_delay = 15
+        self.retry_random_delay = 5
+        self.ssl_verify = ssl_verify
+        self.timeout = float(timeout) if timeout and float(timeout) > 0.0 else None
+        self.throttle_actions = 10
+        self.throttle_commands = 10
+        self.throttle_groups = 10
         self.action_queue = []
         self.local_status = {"multiple-query-count": 0,
                              "single-query-count": 0,
                              "actions-sent": 0,
                              "actions-completed": 0,
                              "actions-queued": 0}
         self.server_status = {"status": "Never contacted",
                               "endpoint": self.endpoint}
-        if auth:
-            self.auth = auth
-        elif auth_dict:
-            self.auth = self._get_auth(ims_host=ims_host, ims_endpoint_jwt=ims_endpoint_jwt, **auth_dict)
-        else:
-            raise ArgumentError("Connector create: either auth (an Auth object) or auth_dict (a dict) is required")
+        self.sync_started = False
+        self.sync_ended = False
         self.session = requests.Session()
         ua_string = "umapi-client/" + umapi_version + " Python/" + python_version() + " (" + platform_version() + ")"
         if user_agent and user_agent.strip():
             ua_string = user_agent.strip() + " " + ua_string
         self.session.headers["User-Agent"] = ua_string
-
-    def _get_auth(self, ims_host, ims_endpoint_jwt,
-                  tech_acct_id=None, api_key=None, client_secret=None,
-                  private_key_file=None, private_key_data=None,
-                  **kwargs):
-        tech_acct_id = tech_acct_id or kwargs.get("tech_acct")
-        private_key_file = private_key_file or kwargs.get("priv_key_path")
-        if not (tech_acct_id and api_key and client_secret and (private_key_data or private_key_file)):
-            raise ArgumentError("Connector create: not all required auth parameters were supplied; please see docs")
-        if private_key_data:
-            jwt = JWT(self.org_id, tech_acct_id, ims_host, api_key, six.StringIO(private_key_data))
-        else:
-            with open(private_key_file, 'r') as private_key_stream:
-                jwt = JWT(self.org_id, tech_acct_id, ims_host, api_key, private_key_stream)
-        token = AccessRequest("https://" + ims_host + ims_endpoint_jwt, api_key, client_secret, jwt())
-        return Auth(api_key, token())
+        self.uuid = str(uuid4())
 
     def status(self, remote=False):
         """
         Return the connection status, both locally and remotely.
 
         The local connection status is a dictionary that gives:
         * the count of multiple queries sent to the server.
@@ -162,24 +168,25 @@
 
         :param remote: whether to query the server for its latest status
         :return: tuple of status dicts: (local, server).
         """
         if remote:
             components = urlparse.urlparse(self.endpoint)
             try:
-                result = self.session.get(components[0] + "://" + components[1] + "/status", timeout=self.timeout)
+                result = self.session.get(components[0] + "://" + components[1] + "/status", timeout=self.timeout,
+                                          verify=self.ssl_verify)
             except Exception as e:
-                if self.logger: self.logger.debug("Failed to connect to server for status: %s", e)
+                self.logger.debug("Failed to connect to server for status: %s", e)
                 result = None
             if result and result.status_code == 200:
                 self.server_status = result.json()
                 self.server_status["endpoint"] = self.endpoint
             elif result:
-                if self.logger: self.logger.debug("Server status response not understandable: Status: %d, Body: %s",
-                                                  result.status_code, result.text)
+                self.logger.debug("Server status response not understandable: Status: %d, Body: %s",
+                             result.status_code, result.text)
                 self.server_status = {"endpoint": self.endpoint,
                                       "status": ("Unexpected HTTP status " + str(result.status_code) + " at: " +
                                                  strftime("%d %b %Y %H:%M:%S +0000", gmtime()))}
             else:
                 self.server_status = {"endpoint": self.endpoint,
                                       "status": "Unreachable at: " + strftime("%d %b %Y %H:%M:%S +0000", gmtime())}
         return self.local_status, self.server_status
@@ -202,63 +209,88 @@
             query_path += "/" + urlparse.quote(component, safe='/@')
         if query_params: query_path += "?" + urlparse.urlencode(query_params)
         try:
             result = self.make_call(query_path)
             body = result.json()
         except RequestError as re:
             if re.result.status_code == 404:
-                if self.logger: self.logger.debug("Ran %s query: %s %s (0 found)",
-                                                  object_type, url_params, query_params)
+                self.logger.debug("Ran %s query: %s %s (0 found)",
+                             object_type, url_params, query_params)
                 return {}
             else:
                 raise re
         if body.get("result") == "success":
             value = body.get(object_type, {})
-            if self.logger: self.logger.debug("Ran %s query: %s %s (1 found)", object_type, url_params, query_params)
+            self.logger.debug("Ran %s query: %s %s (1 found)", object_type, url_params, query_params)
             return value
         else:
             raise ClientError("OK status but no 'success' result", result)
 
     def query_multiple(self, object_type, page=0, url_params=None, query_params=None):
         # type: (str, int, list, dict) -> tuple
         """
         Query for a page of objects.  Defaults to the (0-based) first page.
         Sadly, the sort order is undetermined.
-        :param object_type: string query type (e.g., "users" or "groups")
+        :param object_type: string constant query type: either "user" or "group")
         :param page: numeric page (0-based) of results to get (up to 200 in a page)
         :param url_params: optional list of strings to provide as additional URL components
         :param query_params: optional dictionary of query options
         :return: tuple (list of returned dictionaries (one for each query result), bool for whether this is last page)
         """
-        # Server API convention (v2) is that the pluralized object type goes into the endpoint
-        # and is also the key in the response dictionary for the returned objects.
+        # As of 2017-10-01, we are moving to to different URLs for user and user-group queries,
+        # and these endpoints have different conventions for pagination.  For the time being,
+        # we are also preserving the more general "group" query capability.
         self.local_status["multiple-query-count"] += 1
-        query_type = object_type + "s"  # poor man's plural
-        query_path = "/{}/{}/{:d}".format(query_type, self.org_id, page)
-        for component in url_params if url_params else []:
-            query_path += "/" + urlparse.quote(component)
-        if query_params: query_path += "?" + urlparse.urlencode(query_params)
+        if object_type in ("user", "group"):
+            query_path = "/{}s/{}/{:d}".format(object_type, self.org_id, page)
+            if url_params: query_path += "/" + "/".join([urlparse.quote(c) for c in url_params])
+            if query_params: query_path += "?" + urlparse.urlencode(query_params)
+        elif object_type == "user-group":
+            query_path = "/{}/user-groups".format(self.org_id)
+            if url_params: query_path += "/" + "/".join([urlparse.quote(c) for c in url_params])
+            query_path += "?page={:d}".format(page+1)
+            if query_params: query_path += "&" + urlparse.urlencode(query_params)
+        else:
+            raise ArgumentError("Unknown query object type ({}): must be 'user' or 'group'".format(object_type))
         try:
             result = self.make_call(query_path)
             body = result.json()
         except RequestError as re:
             if re.result.status_code == 404:
-                if self.logger: self.logger.debug("Ran %s query: %s %s (0 found)",
-                                                  object_type, url_params, query_params)
-                return [], True
+                self.logger.debug("Ran %s query: %s %s (0 found)",
+                             object_type, url_params, query_params)
+                return [], True, 0, 0, 0, 0
             else:
                 raise re
-        if body.get("result") == "success":
-            values = body.get(query_type, [])
-            last_page = body.get("lastPage", False)
-            if self.logger: self.logger.debug("Ran multi-%s query: %s %s (page %d: %d found)",
-                                              object_type, url_params, query_params, page, len(values))
-            return values, last_page
+
+        headers = {k.lower(): v for k, v in result.headers.items()}
+        total_count = headers.get("x-total-count", "0")
+        page_count = headers.get("x-page-count", "0")
+        page_number = headers.get("x-current-page", "1")
+        page_size = headers.get("x-page-size", "0")
+
+        if object_type in ("user", "group"):
+            if body.get("result") == "success":
+                values = body.get(object_type + "s", [])
+                last_page = body.get("lastPage", False)
+
+                self.logger.debug("Ran multi-%s query: %s %s (page %d: %d found)",
+                             object_type, url_params, query_params, page, len(values))
+                return values, last_page, int(total_count), int(page_count), int(page_number), int(page_size)
+            else:
+                raise ClientError("OK status but no 'success' result", result)
+        elif object_type == "user-group":
+            self.logger.debug("Ran multi-group query: %s %s (page %d: %d found)",
+                         url_params, query_params, page, len(body))
+            return body, int(page_number) >= int(page_count), int(total_count), int(page_count), \
+                   int(page_number), int(page_size)
         else:
-            raise ClientError("OK status but no 'success' result", result)
+            # this would actually be caught above, but we use a parallel construction in both places
+            # to make it easy to add query object types
+            raise ArgumentError("Unknown query object type ({}): must be 'user' or 'group'".format(object_type))
 
     def execute_single(self, action, immediate=False):
         """
         Execute a single action (containing commands on a single object).
         Normally, since actions are batched so as to be most efficient about execution,
         but if you want this command sent immediately (and all prior queued commands
         sent earlier in this command's batch), specify a True value for the immediate flag.
@@ -283,15 +315,15 @@
         return self.execute_multiple([], immediate=True)
 
     def execute_multiple(self, actions, immediate=True):
         """
         Execute multiple Actions (each containing commands on a single object).
         Normally, the actions are sent for execution immediately (possibly preceded
         by earlier queued commands), but if you are going for maximum efficiency
-        you can set immeediate=False which will cause the connection to wait
+        you can set immediate=False which will cause the connection to wait
         and batch as many actions as allowed in each server call.
 
         Since any command can fill the current batch, one or more of your commands may be submitted
         even if you don't specify the immediate flag.  So don't think of this call as always
         being a queue call when immedidate=False.
 
         Returns the number of actions left in the queue, that got sent, and that executed successfully.
@@ -309,50 +341,60 @@
         """
         # throttling part 1: split up each action into smaller actions, as needed
         # optionally split large lists of groups in add/remove commands (if action supports it)
         split_actions = []
         exceptions = []
         for a in actions:
             if len(a.commands) == 0:
-                if self.logger: self.logger.warning("Sending action with no commands: %s", a.frame)
+                self.logger.warning("Sending action with no commands: %s", a.frame)
             # maybe_split_groups is a UserAction attribute, so the call may throw an AttributeError
             try:
                 if a.maybe_split_groups(self.throttle_groups):
-                    if self.logger: self.logger.debug(
+                    self.logger.debug(
                         "Throttling actions %s to have a maximum of %d entries in group lists.",
                         a.frame, self.throttle_groups)
             except AttributeError:
                 pass
             if len(a.commands) > self.throttle_commands:
-                if self.logger: self.logger.debug("Throttling action %s to have a maximum of %d commands.",
+                self.logger.debug("Throttling action %s to have a maximum of %d commands.",
                                                   a.frame, self.throttle_commands)
                 split_actions += a.split(self.throttle_commands)
             else:
                 split_actions.append(a)
         actions = self.action_queue + split_actions
         # throttling part 2: execute the action list in batches, as needed
         sent = completed = 0
         batch_size = self.throttle_actions
         min_size = 1 if immediate else batch_size
         while len(actions) >= min_size:
             batch, actions = actions[0:batch_size], actions[batch_size:]
-            if self.logger: self.logger.debug("Executing %d actions (%d remaining).", len(batch), len(actions))
+            self.logger.debug("Executing %d actions (%d remaining).", len(batch), len(actions))
             sent += len(batch)
             try:
                 completed += self._execute_batch(batch)
             except Exception as e:
                 exceptions.append(e)
         self.action_queue = actions
         self.local_status["actions-queued"] = queued = len(actions)
         self.local_status["actions-sent"] += sent
         self.local_status["actions-completed"] += completed
         if exceptions:
             raise BatchError(exceptions, queued, sent, completed)
         return queued, sent, completed
 
+    def start_sync(self):
+        """Signal the beginning of a sync operation
+        Sends a header with the first batch of UMAPI actions"""
+        self.sync_started = True
+
+    def end_sync(self):
+        """Signal the end of a sync operation
+        Sends a header with the next batch of UMAPI actions"""
+        self.sync_ended = True
+
     def _execute_batch(self, actions):
         """
         Execute a single batch of Actions.
         For each action that has a problem, we annotate the action with the
         error information for that action, and we return the number of
         successful actions in the batch.
         :param actions: the list of Action objects to be executed
@@ -362,79 +404,88 @@
         if self.test_mode:
             result = self.make_call("/action/%s?testOnly=true" % self.org_id, wire_form)
         else:
             result = self.make_call("/action/%s" % self.org_id, wire_form)
         body = result.json()
         if body.get("errors", None) is None:
             if body.get("result") != "success":
-                if self.logger: self.logger.warning("Server action result: no errors, but no success:\n%s", body)
+                self.logger.warning("Server action result: no errors, but no success:\n%s", body)
             return len(actions)
         try:
             if body.get("result") == "success":
-                if self.logger: self.logger.warning("Server action result: errors, but success report:\n%s", body)
+                self.logger.warning("Server action result: errors, but success report:\n%s", body)
             for error in body["errors"]:
                 actions[error["index"]].report_command_error(error)
         except:
             raise ClientError(str(body), result)
         return body.get("completed", 0)
 
-    def make_call(self, path, body=None):
+    def make_call(self, path, body=None, delete=False):
         """
         Make a single UMAPI call with error handling and retry on temporary failure.
         :param path: the string endpoint path for the call
         :param body: (optional) list of dictionaries to be serialized into the request body
         :return: the requests.result object (on 200 response), raise error otherwise
         """
+        extra_headers = {"X-Request-Id": f"{self.uuid}_{int(datetime.now().timestamp()*1000)}"}
+        # if the sync_started or sync_ended flags are set, send a header for any type of call
+        if self.sync_started:
+            self.logger.info("Sending start_sync signal")
+            extra_headers['Pragma'] = 'umapi-sync-start'
+            self.sync_started = False
+        elif self.sync_ended:
+            self.logger.info("Sending end_sync signal")
+            extra_headers['Pragma'] = 'umapi-sync-end'
+            self.sync_ended = False
         if body:
             request_body = json.dumps(body)
-
             def call():
-                return self.session.post(self.endpoint + path, auth=self.auth, data=request_body, timeout=self.timeout)
+                return self.session.post(self.endpoint + path, auth=self.auth, data=request_body, timeout=self.timeout,
+                                         verify=self.ssl_verify, headers=extra_headers)
         else:
-            def call():
-                return self.session.get(self.endpoint + path, auth=self.auth, timeout=self.timeout)
+            if not delete:
+                def call():
+                    return self.session.get(self.endpoint + path, auth=self.auth, timeout=self.timeout,
+                                            verify=self.ssl_verify, headers=extra_headers)
+            else:
+                def call():
+                    return self.session.delete(self.endpoint + path, auth=self.auth, timeout=self.timeout,
+                                               verify=self.ssl_verify, headers=extra_headers)
 
         start_time = time()
         result = None
         for num_attempts in range(1, self.retry_max_attempts + 1):
+            checked_result = None
             try:
                 result = call()
-                if result.status_code == 200:
-                    return result
-                elif result.status_code in [429, 502, 503, 504]:
-                    if self.logger: self.logger.warning("UMAPI timeout...service unavailable (code %d on try %d)",
-                                                        result.status_code, num_attempts)
-                    retry_wait = 0
-                    if "Retry-After" in result.headers:
-                        advice = result.headers["Retry-After"]
-                        advised_time = parsedate_tz(advice)
-                        if advised_time is not None:
-                            # header contains date
-                            retry_wait = int(mktime_tz(advised_time) - time())
-                        else:
-                            # header contains delta seconds
-                            retry_wait = int(advice)
-                    if retry_wait <= 0:
-                        # use exponential back-off with random delay
-                        delay = randint(0, self.retry_random_delay)
-                        retry_wait = (int(pow(2, num_attempts - 1)) * self.retry_first_delay) + delay
-                elif 201 <= result.status_code < 400:
-                    raise ClientError("Unexpected HTTP Status {:d}: {}".format(result.status_code, result.text), result)
-                elif 400 <= result.status_code < 500:
-                    raise RequestError(result)
-                else:
-                    raise ServerError(result)
+                checked_result = APIResult(result).check_result()
             except requests.Timeout:
-                if self.logger: self.logger.warning("UMAPI connection timeout...(%d seconds on try %d)",
-                                                    self.timeout, num_attempts)
-                retry_wait = 0
-                result = None
+                self.logger.warning("UMAPI connection timeout...(%d seconds on try %d)",
+                               self.timeout, num_attempts)
+                checked_result = APIResult(success=False, timeout=0)
+            except requests.ConnectionError:
+                self.logger.warning("UMAPI connection error...(%d seconds on try %d)",
+                               self.timeout, num_attempts)
+                checked_result = APIResult(success=False, timeout=0)
+            
+            if checked_result.success:
+                return result
+
+            self.logger.warning("UMAPI request limit reached (code %s on try %d)",
+                           checked_result.status_code, num_attempts)
+
+            retry_wait = checked_result.timeout
+            if retry_wait <= 0:
+                # use exponential back-off with random delay
+                delay = randint(0, self.retry_random_delay)
+                retry_wait = (int(pow(2, num_attempts - 1)) * self.retry_first_delay) + delay
+
             if num_attempts < self.retry_max_attempts:
                 if retry_wait > 0:
-                    if self.logger: self.logger.warning("Next retry in %d seconds...", retry_wait)
+                    self.logger.warning("waiting %d seconds to continue...", retry_wait)
                     sleep(retry_wait)
                 else:
-                    if self.logger: self.logger.warning("Immediate retry...")
+                    self.logger.warning("Immediate retry...")
         total_time = int(time() - start_time)
-        if self.logger: self.logger.error("UMAPI timeout...giving up after %d attempts (%d seconds).",
-                                          self.retry_max_attempts, total_time)
-        raise UnavailableError(self.retry_max_attempts, total_time, result)
+        self.logger.error("UMAPI timeout...giving up after %d attempts (%d seconds).",
+                     self.retry_max_attempts, total_time)
+        raise UnavailableError(self.retry_max_attempts, total_time, checked_result.result)
```

### Comparing `umapi-client-2.9/umapi_client/error.py` & `umapi_client-3.0/umapi_client/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2016-2017 Adobe Systems Incorporated.  All rights reserved.
+# Copyright (c) 2016-2021 Adobe Inc.  All rights reserved.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -14,16 +14,14 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import six
-
 
 class UnavailableError(Exception):
     def __init__(self, attempts, seconds, result):
         Exception.__init__(self, "Server unavailable: Made {:d} attempts over {:d} seconds".format(attempts, seconds))
         self.attempts = attempts
         self.seconds = seconds
         self.result = result
@@ -54,10 +52,13 @@
         Exception.__init__(self, prefix + tail)
         self.causes = causes
         self.statistics = (queued, sent, completed)
 
 
 class ArgumentError(ValueError):
     def __init__(self, message):
-        if six.PY2 and isinstance(message, unicode):
-            message = message.encode('utf8')
         ValueError.__init__(self, message)
+
+
+class UnsupportedError(Exception):
+    def __init__(self, message):
+        Exception.__init__(self, "Unsupported Feature Error: " + message)
```

### Comparing `umapi-client-2.9/umapi_client/version.py` & `umapi_client-3.0/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Copyright (c) 2016-2017 Adobe Systems Incorporated.  All rights reserved.
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
+MIT License
 
-__version__ = "2.9"
+Copyright (c) 2016-2021 Adobe Inc.  All rights reserved.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

