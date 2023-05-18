# Comparing `tmp/revproxy_auth-0.0.9.tar.gz` & `tmp/revproxy_auth-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revproxy_auth-0.0.9.tar", last modified: Fri Apr 14 07:04:15 2023, max compression
+gzip compressed data, was "revproxy_auth-0.1.0.tar", last modified: Thu May 18 12:11:04 2023, max compression
```

## Comparing `revproxy_auth-0.0.9.tar` & `revproxy_auth-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/revproxy_auth/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/config-template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/revproxy_auth/cookies/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/revproxy_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.663046 revproxy_auth-0.0.9/revproxy_auth/revproxy_auth_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/revproxy_auth/revproxy_auth_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/revproxy_auth_static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/revproxy_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/revproxy_auth/templates/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/revproxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-14 07:04:15.000000 revproxy_auth-0.0.9/revproxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-14 07:04:15.000000 revproxy_auth-0.0.9/revproxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:04:15.000000 revproxy_auth-0.0.9/revproxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 07:04:15.000000 revproxy_auth-0.0.9/revproxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 07:04:15.000000 revproxy_auth-0.0.9/revproxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:04:15.667046 revproxy_auth-0.0.9/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/tests/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25649 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/tests/data/test_result
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-14 07:04:07.000000 revproxy_auth-0.0.9/tests/test_000.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/revproxy_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/revproxy_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/revproxy_auth/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17779 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/revproxy_auth/revproxy_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/revproxy_auth/revproxy_auth_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/revproxy_auth/revproxy_auth_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/revproxy_auth/revproxy_auth_static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/revproxy_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/revproxy_auth/templates/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/revproxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-18 12:11:04.000000 revproxy_auth-0.1.0/revproxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 12:11:04.000000 revproxy_auth-0.1.0/revproxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:11:04.000000 revproxy_auth-0.1.0/revproxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 12:11:04.000000 revproxy_auth-0.1.0/revproxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 12:11:04.000000 revproxy_auth-0.1.0/revproxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:11:04.300763 revproxy_auth-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:04.296763 revproxy_auth-0.1.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/tests/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25649 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/tests/data/test_result
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-18 12:10:50.000000 revproxy_auth-0.1.0/tests/test_001.py
```

### Comparing `revproxy_auth-0.0.9/PKG-INFO` & `revproxy_auth-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy_auth
-Version: 0.0.9
+Version: 0.1.0
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # Authproxy
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.0.9/README.md` & `revproxy_auth-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.0.9/revproxy_auth/revproxy_auth.py` & `revproxy_auth-0.1.0/revproxy_auth/revproxy_auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,120 @@
 """ Class to perform authentication using the synology authmethods """
 import os
 import time
 from urllib import parse
 import json
 from pathlib import Path
 import secrets
-from typing import Union
 import jinja2
 import requests
-from flask import request, Response, send_from_directory
+from flask import Flask, request, Response, send_from_directory, redirect
 
 from config_yml import Config
 
 COOKIE_LIFE_MINUTES = 15
 
-class ApiRestResponse():
-    """ Api Rest reponse data, platform (flask) independent"""
-    def __init__(self, content: str,
-                 set_cookies: dict=None,
-                 delete_cookies: dict=None,
-                 created_local_cookies: dict=None,
-                 status: int=200,
-                 content_type: str='application/octet-stream') -> None:
-        self.content = content
-        self.set_cookies = {} if not set_cookies else set_cookies
-        self.delete_cookies = {} if not delete_cookies else delete_cookies
-        self.status = status
-        self.content_type = content_type
-        self.created_local_cookies = {} if not created_local_cookies else created_local_cookies
+HTTP_200_OK = 200
+HTTP_501_NOT_IMPLEMENTED = 501
 
 class RevProxyAuth():
     """ 
     Class to manage the authentication. 
     The path_redirect function should be called from a '/<path:path>' flask rule
     Also a rule '/' should call this function like this:  return self.auth_proxy.path_redirect("/")
     """
-    def __init__(self, template_config_path: str=None) -> None:
+    def __init__(self, app: Flask,
+                 root_class: str='revproxy_auth',
+                 template_config_path: str=None,
+                 dry_run=False) -> None:
         """
             template_config_path: full path of configuration template
         """
 
         if not template_config_path:
             template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
-        self._config = Config('authproxy', template_config_path, 'config.yml')
+        self._config = Config(root_class, template_config_path, 'revproxy_auth_config.yml', dry_run=dry_run)
 
-        self.cookie_folder = os.path.join(Path(__file__).parent.resolve(), 'cookies')
+        self.homevar = os.path.join(str(Path.home()), 'var', root_class)
+
+        self.auth_cookie_folder = os.path.join(self.homevar, 'auth_cookies')
+        if not os.path.exists(self.auth_cookie_folder):
+            os.makedirs(self.auth_cookie_folder)
+        self.session_cookie_folder = os.path.join(self.homevar, 'session_cookies')
+        if not os.path.exists(self.session_cookie_folder):
+            os.makedirs(self.session_cookie_folder)
+        self.app = app
+        self.app.add_url_rule(rule='/revproxy_auth_static/<path:path>',
+                              view_func=self._get_static_content,
+                              methods=['GET', 'POST'])
+
+    def token_valid(self, req):
+        """ Checks if the token in the request matches an existing and not-expired cookie file
+        Args:
+            req (Request): Http request
+        Returns:
+            bool: True if token matches cookie file, and its not expired yet
+        """
+        valid = False
+        cookie_name = req.cookies.get('token', None)
+        if cookie_name:  # We get a token... lets verify if its legitimate, and still alive
+            valid = not self._clear_local_cookie_if_expired(self.auth_cookie_folder, cookie_name)
+        return valid
+
+    def get_auth_response(self, req, callback) -> Response:
+        """ If valid auth token comes fromt he client, return none
+            Otherwise, it will return a response so that the client opens again the Auth Popup
+        Returns:
+            Response: Http response with the auth popup, or 
+                      None if auth request is not needed because already are authenticated
+        """
+        response = None
+        # Try to get authentication from the cookie
+        cookie_name = req.cookies.get('token', None)
+        print(f'Incomming Session token Cookie name: {cookie_name}')
+
+        if cookie_name and not req.form.get('auth', None):
+            # We get a session token... lets verify if its legitimate, and still alive
+            cookie = self._get_local_session_cookie(cookie_name)
+            if cookie: # Already authenticated --> Lets tunnel info back to client
+                print(f'AUTHENTICATED: Session Token Cookie {cookie_name} exists in local')
+                response = callback()
+            else: # We got a session, but its no longer valid --> ask again for credentials
+                print(f'NOT AUTHENTICATED: Session Token Cookie {cookie_name} DOESNT exist in local')
+                response = self._reask_credentials(self._get_request_dict(req.path), old_cookie_name=cookie_name)
+        else:  # Not authenticated yet... Two options:
+               # 1) We have to pop the authentication popup to the user
+               # 2) We already did, and we need to look for the auth info in the form to verify it
+            print('Not authenticated yet')
+            request_dict = self._get_request_dict(req.path)
+            session_cookie, session_cookie_name = self._auth_from_popup_data(request_dict)
+            if session_cookie_name:
+                # To get rid of the POST form data, and reenter with the valid session token
+                response = redirect(session_cookie['endpoint'])
+                response.set_cookie('token', session_cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
+            else:
+                response = self._reask_credentials(request_dict)
+
+        return response
 
     def path_redirect(self, path) -> Response:
         """Main entry point
         Returns:
             http_response: response string
         """
         print(f'---------------------- Path requested: {path} --------------------')
+        resp = self._path_redirect(self._get_request_dict(path))
+        return resp
 
-        request_dict = {'host': request.host,
-                        'endpoint': path,
-                        'method': request.method,
-                        'params': request.query_string.decode("utf-8"),
-                        'data': request.get_data(),
-                        'headers': request.headers,
-                        'cookies': request.cookies,
-                        'form': request.form
-                        }
-
-        resp = self._path_redirect(request_dict)
-
-        if isinstance(resp, ApiRestResponse):
-            flask_response = Response(resp.content, status=resp.status, content_type=resp.content_type)
-            if resp.delete_cookies:
-                for del_cookie, domain in resp.delete_cookies.items():
-                    flask_response.delete_cookie(del_cookie, domain)
-            if resp.set_cookies:
-                for set_cookie, value in resp.set_cookies.items():
-                    flask_response.set_cookie(set_cookie, value, max_age=COOKIE_LIFE_MINUTES*60)
-
-            return flask_response
-        else:
-            return resp
-
-    def _build_cookie(self, req_dict: dict) -> tuple:
+    def _build_auth_cookie(self, req_dict: dict) -> tuple:
         mapping_info = self._config['mapping'].get(req_dict['host'])
+        if not mapping_info:
+            return None, None
+
         host = mapping_info.get('host')
         endpoint = mapping_info.get('endpoint')
         method = mapping_info.get('method')
         params = req_dict['params']
 
         ser_head = {}
         for head in req_dict['headers']:
@@ -99,137 +129,214 @@
                   'method': method,
                   'params': params, 
                   'headers': headers,
                   'content': content}
 
         return cookie, cookie_name
 
-    def _write_cookie(self, cookie: dict, cookie_name: str):
-        cookie_path = os.path.join(self.cookie_folder, cookie_name)
+    def _build_session_cookie(self, auth_cookie: dict) -> tuple:
+        cookie = {'session': True,
+                  'endpoint': parse.urljoin(auth_cookie['host'], auth_cookie['endpoint'])
+                 }
+        return cookie, secrets.token_urlsafe(16)
+
+    def _get_request_dict(self, endpoint):
+        return {'host': request.host,
+                'endpoint': endpoint,
+                'method': request.method,
+                'params': request.query_string.decode("utf-8"),
+                'data': request.get_data(),
+                'headers': request.headers,
+                'cookies': request.cookies,
+                'form': request.form
+               }
+
+    def _get_static_content(self, path: str):
+        """Get revproxy_auth custom static content
+        Args:
+            path (str): Resource to be retrieved from revproxy_aut_static folder
+
+        Returns:
+            _type_: Resouce
+        """
+        full_path = os.path.join(Path(__file__).parent.resolve(), 'revproxy_auth_static')
+        return send_from_directory(full_path, path)
+
+    def _write_cookie(self, cookie: dict, cookie_folder: str, cookie_name: str):
+        self._clear_expired_cookies(cookie_folder) # Housekeeping before writting new
+
+        cookie_path = os.path.join(cookie_folder, cookie_name)
         with open(cookie_path, 'w', encoding="utf-8") as cookie_file:
             json.dump(cookie, cookie_file)
 
-    def _clear_expired_cookies(self):
-        for filename in os.listdir(self.cookie_folder):
-            filepath = os.path.join(self.cookie_folder, filename)
-            # checking if it is a file
-            if os.path.isfile(filepath):
-                age = time.time() - os.path.getmtime(filepath)
-                if age > COOKIE_LIFE_MINUTES*60:
-                    os.remove(filepath)
+    def _clear_local_cookie(self, cookie_folder: str, cookie_name: str):
+        cleared = False
+        cookie_file_name = os.path.join(cookie_folder, cookie_name)
+        if os.path.isfile(cookie_file_name):
+            cleared = True
+            os.remove(cookie_file_name)
+        return cleared
+
+    def _clear_local_cookie_if_expired(self, cookie_folder: str, cookie_name: str):
+        cleared = False
+        cookie_file_name = os.path.join(cookie_folder, cookie_name)
+        if os.path.isfile(cookie_file_name):
+            age = time.time() - os.path.getmtime(cookie_file_name)
+            if age > COOKIE_LIFE_MINUTES*60:
+                cleared = True
+                os.remove(cookie_file_name)
+        return cleared
+
+    def _clear_expired_cookies(self, cookie_folder: str):
+        for filename in os.listdir(cookie_folder):
+            self._clear_local_cookie_if_expired(cookie_folder, filename)
 
-    def _build_auth_popup(self, cookie_name: str) -> ApiRestResponse:
+    def _build_auth_popup(self, cookie_name: str) -> Response:
         # Get the auth html form template and send back to the user, so he can authenticate
         form_path = os.path.join(Path(__file__).parent.resolve(), 'templates', 'form.html')
         with open(form_path, 'r', encoding="utf8") as form:
             buff = form.read()
             # replace the cookie name
             env = jinja2.Environment()
             template = env.from_string(buff)
-            content = template.render(token=cookie_name)
-            return ApiRestResponse(content, content_type='text/html')
+            content = template.render(auth=cookie_name)
+            return Response(content, status=HTTP_200_OK,  content_type='text/html')
 
-    def _get_local_cookie(self, token:str = None):
+    def _get_local_auth_cookie(self, cookie_name:str = None):
         cookie = None
-        if token:
-            cookie_path = os.path.join(self.cookie_folder, token)
+        if cookie_name:
+            cookie_path = os.path.join(self.auth_cookie_folder, cookie_name)
             if os.path.exists(cookie_path):
                 with open(cookie_path, 'r', encoding="utf-8") as cookie_file:
                     cookie = json.load(cookie_file)
 
                     cookie['headers'] = json.loads(cookie['headers'])
         return cookie
 
+    def _get_local_session_cookie(self, cookie_name:str = None):
+        cookie = None
+        if cookie_name:
+            cookie_path = os.path.join(self.session_cookie_folder, cookie_name)
+            if os.path.exists(cookie_path):
+                with open(cookie_path, 'r', encoding="utf-8") as cookie_file:
+                    cookie = json.load(cookie_file)
+        return cookie
+
     def _credentials_valid(self, form):
-        token = form.get('token', None)
+        token = form.get('auth', None)
         if token:
-            user = form.get('user', None)
-            password = form.get('password', None)
-            otp = form.get('OTP', None)
-            url = (f'{self._config["NAS"]}/webapi/entry.cgi?api=SYNO.API.Auth&version=6&method=login'
-                   f'&account={user}&passwd={password}&otp_code={otp}')
-            auth_response = requests.get(url, timeout=10)
-            # Verify authentication
-            return auth_response.json()['success']
+            user = form.get('user', '').strip(' \t\n\r')
+            password = form.get('password', '').strip(' \t\n\r')
+            otp = form.get('OTP', '').strip(' \t\n\r')
+            testing_credentials = self._config['testing_credentials']
+            if not testing_credentials:
+                url = (f'{self._config["NAS"]}/webapi/entry.cgi?api=SYNO.API.Auth&version=6&method=login'
+                       f'&account={user}&passwd={password}&otp_code={otp}')
+                auth_response = requests.get(url, timeout=10)
+                # Verify authentication
+                return auth_response.json()['success']
+            else: # Testing credentiales
+                return user == testing_credentials['user'] and \
+                       password == testing_credentials['password'] and \
+                       otp == testing_credentials['OTP']
         return False
 
-    def _call_inner_get(self, host, endpoint, params, headers) -> ApiRestResponse:
+    def _call_inner_get(self, host, endpoint, params, headers) -> Response:
         fullpath = parse.urljoin(host, endpoint)
         resp = requests.get(fullpath,
                             params=params,
                             headers = headers,
                             timeout=10)
-        return ApiRestResponse(resp.text, status=resp.status_code, content_type=resp.headers['content-type'])
+        return Response(resp.text, status=resp.status_code, content_type=resp.headers['content-type'])
 
-    def _call_inner_post(self, host, endpoint, data, headers) -> ApiRestResponse:
+    def _call_inner_post(self, host, endpoint, data, headers) -> Response:
         fullpath = parse.urljoin(host, endpoint)
         resp = requests.post(fullpath,
                              data = data,
                              headers = headers,
                              timeout=10)
-        return ApiRestResponse(resp.text, status=resp.status_code, content_type=resp.headers['content-type'])
+        return Response(resp.text, status=resp.status_code, content_type=resp.headers['content-type'])
 
-    def _reask_credentials(self, request_dict: dict, old_cookie_name: str = None) -> ApiRestResponse:
-        new_cookie, new_cookie_name = self._build_cookie(request_dict)
-        self._clear_expired_cookies() # Housekeeping
-        print(f'Creating new cookie {new_cookie_name}')
-        self._write_cookie(new_cookie, new_cookie_name)
+    def _reask_credentials(self, request_dict: dict, old_cookie_name: str = None) -> Response:
+        new_cookie, new_cookie_name = self._build_auth_cookie(request_dict)
+        if not new_cookie: # Unable to build cookie for requested path: host unknown
+            return Response(request_dict['host'], status=HTTP_501_NOT_IMPLEMENTED, content_type='text/plain')
+            # return ApiRestResponse(request_dict['host'], status=501)
+        print(f'Creating new auth cookie {new_cookie_name} and reasking to user...')
+        self._write_cookie(new_cookie, self.auth_cookie_folder, new_cookie_name)
         response = self._build_auth_popup(new_cookie_name)
-        response.created_local_cookies[new_cookie_name] = new_cookie
+        # response.set_cookie('auth', new_cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
         if old_cookie_name:
-            response.delete_cookies['token'] = request_dict['host']
             print(f'Deleting cookie in response: {old_cookie_name}')
-            # response.delete_cookie('token', request_dict['host'])
+            response.delete_cookie('auth',  request_dict['host'])
+            self._clear_local_cookie(self.auth_cookie_folder, old_cookie_name)
         return response
 
-    def _first_auth_and_redirect(self, request_dict) -> ApiRestResponse:
-        cookie_name = request_dict['form'].get('token', None) if request_dict['form'].get('from_auth') else None
-        cookie = self._get_local_cookie(cookie_name)
+    def _auth_from_popup_data(self, request_dict) -> str:
+        session_cookie_name = None
+        session_cookie = None
+        # cookie_name = request_dict['form'].get('token', None) if request_dict['form'].get('from_auth') else None
+        cookie_name = request_dict['form'].get('auth', None)
+        auth_cookie = self._get_local_auth_cookie(cookie_name)
+        if auth_cookie:
+            if self._credentials_valid(request_dict['form']):
+                print(f'Auth Local cookie {cookie_name} still alive and valid.')
+                session_cookie, session_cookie_name = self._build_session_cookie(auth_cookie)
+                print(f'Creating new session cookie {session_cookie_name} and reasking to user...')
+                self._write_cookie(session_cookie, self.session_cookie_folder, session_cookie_name)
+            else:
+                print(f'Auth Local cookie {cookie_name} still alive but credentials are invalid.')
+        else:
+            print(f'Auth Local cookie {cookie_name} doesnt exist.')
+        return session_cookie, session_cookie_name
+
+    def _first_auth_and_redirect(self, request_dict) -> Response:
+        cookie_name = request_dict['form'].get('auth', None)
+        cookie = self._get_local_auth_cookie(cookie_name)
         if cookie:
             print(f'Local cookie {cookie_name} still alive')
             if self._credentials_valid(request_dict['form']):
                 print('Credentials validated by synology NAS')
                 # Search for the cookie and redirect to related URL if present
                 if cookie['method'] == 'GET':
                     response = self._call_inner_get(cookie['host'], cookie['endpoint'], cookie['params'], {})
                 else:
                     response = self._call_inner_post(cookie['host'], cookie['endpoint'], cookie['content'], {})
-                response.set_cookies['token'] = cookie_name
-                # response.set_cookie('token', cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
+                response.set_cookie('token', cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
             else: # We come from the auth popup, but credentials are invalid --> ask again for credentials
                 print('Credentials rejected by synology NAS. Reopening auth popup')
                 response = self._build_auth_popup(cookie_name)
         else: # We got a token, but its no longer valid --> ask again for credentials
             print('Local cookie expired. Reopening auth popup')
             response = self._reask_credentials(request_dict, cookie_name)
         return response
 
-
-    def _path_redirect(self, request_dict) -> Union[ApiRestResponse, Response]:
+    def _path_redirect(self, request_dict) -> Response:
         """ Flask independent internal function
         Returns:
             http_response: response string
         """
         if request_dict['endpoint'] == 'favicon.ico':
-            cookie, cookie_name = self._build_cookie(request_dict)
+            cookie, cookie_name = self._build_auth_cookie(request_dict)
+            if not cookie: # Unable to build cookie for requested path: host unknown
+                return Response(request_dict['host'], status=501, content_type='text/plain')
             print(f"favicon.ico requested: Directly returning from inner endpoint {cookie['host']}")
             return self._call_inner_get(host=cookie['host'],
                                         endpoint=request_dict['endpoint'],
                                         params=request_dict['params'],
                                         headers=request_dict['headers'])
 
         if request_dict['endpoint'].startswith('revproxy_auth_static'):
-            full_path = os.path.join(Path(__file__).parent.resolve())
-            return send_from_directory(full_path, request_dict['endpoint'])
+            return self._get_static_content(request_dict['endpoint'])
 
         # Try to get authentication from the cookie
         cookie_name = request_dict['cookies'].get('token', None)
         print(f'Incomming Cookie name: {cookie_name}')
         if cookie_name:  # We get a token... lets verify if its legitimate, and still alive
-            cookie = self._get_local_cookie(cookie_name)
+            cookie = self._get_local_session_cookie(cookie_name)
             if cookie: # Already authenticated --> Lets tunnel info back to client
                 print(f'AUTHENTICATED: Cookie {cookie_name} exists in local')
                 if request_dict['endpoint'] == '/': # If path is the root, lets go to the configured initial entrypoint.
                     method = cookie['method']
                     path = cookie['endpoint']
                     headers = {}
                     if method == 'GET':
```

### Comparing `revproxy_auth-0.0.9/revproxy_auth/revproxy_auth_static/css/view.css` & `revproxy_auth-0.1.0/revproxy_auth/revproxy_auth_static/css/view.css`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.0.9/revproxy_auth/templates/form.html` & `revproxy_auth-0.1.0/revproxy_auth/templates/form.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!--authproxy-->
 <html xmlns="http://www.w3.org/1999/xhtml">
 <head>
 <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
-<meta name="viewport" content="width-device-width, initial-scale=1.0">
+<meta name="viewport" content="width=device-width, initial-scale=1.0">
 <link rel="stylesheet" type="text/css" href="revproxy_auth_static/css/view.css" media="all">
 <title>Login with Synology Auth</title>
 </head>
 <body id="main_body">
   <div id="form_container">
     <form id="signin_form" style=" margin-block-end: 0em;" method="POST">
             <h1>Sign in</h1>
@@ -18,13 +18,12 @@
             </div>
             <div style="margin: 1px">
                 <input name = "OTP" type="text" placeholder="OTP Code" class="edit_text">
             </div>
             <div style="margin: 1px">
                 <input type="submit" value="Sign in" class="button_text">
             </div>
-            <input name = "token" type="hidden" value="{{token}}">
-            <input name = "from_auth" type="hidden" value="True">
+            <input name = "auth" type="hidden" value="{{auth}}" id="auth">
         </form>  
   </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,7 @@
 
 
 ****** Sign in ******
 [user                ]
 [********************]
 [OTP                 ]
 [Sign in]
-
```

### Comparing `revproxy_auth-0.0.9/revproxy_auth.egg-info/PKG-INFO` & `revproxy_auth-0.1.0/revproxy_auth.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy-auth
-Version: 0.0.9
+Version: 0.1.0
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # Authproxy
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.0.9/setup.py` & `revproxy_auth-0.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="revproxy_auth",
-    version="0.0.9",
+    version="0.1.0",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Reverse proxy with synology authentication",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/revproxy_auth",
     packages=setuptools.find_packages(),
@@ -26,11 +26,12 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Home Automation"
     ],
     install_requires=[
         'Flask>=1.1.2',
-        'config_yml>=0.2.0'
+        'config_yml>=0.3.0',
+        'beautifulsoup4>=4.10.0'
     ],
     python_requires='>=3.6',
 )
```

### Comparing `revproxy_auth-0.0.9/tests/data/test_result` & `revproxy_auth-0.1.0/tests/data/test_result`

 * *Files identical despite different names*

