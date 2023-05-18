# Comparing `tmp/saleor-social-auth-0.5.0.tar.gz` & `tmp/saleor-social-auth-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saleor-social-auth-0.5.0.tar", last modified: Wed Oct 19 07:57:51 2022, max compression
+gzip compressed data, was "saleor-social-auth-0.6.0.tar", last modified: Thu May 18 15:55:16 2023, max compression
```

## Comparing `saleor-social-auth-0.5.0.tar` & `saleor-social-auth-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ace        (502) staff       (20)        0 2022-10-19 07:57:51.598917 saleor-social-auth-0.5.0/
--rw-r--r--   0 ace        (502) staff       (20)     1064 2021-08-17 07:53:44.000000 saleor-social-auth-0.5.0/LICENSE
--rw-r--r--   0 ace        (502) staff       (20)     1911 2022-10-19 07:57:51.598693 saleor-social-auth-0.5.0/PKG-INFO
--rw-r--r--   0 ace        (502) staff       (20)     1321 2022-02-09 09:02:49.000000 saleor-social-auth-0.5.0/README.md
--rw-r--r--   0 ace        (502) staff       (20)      231 2021-08-17 07:53:44.000000 saleor-social-auth-0.5.0/pyproject.toml
-drwxr-xr-x   0 ace        (502) staff       (20)        0 2022-10-19 07:57:51.593861 saleor-social-auth-0.5.0/saleor_social_auth.egg-info/
--rw-r--r--   0 ace        (502) staff       (20)     1911 2022-10-19 07:57:51.000000 saleor-social-auth-0.5.0/saleor_social_auth.egg-info/PKG-INFO
--rw-r--r--   0 ace        (502) staff       (20)      443 2022-10-19 07:57:51.000000 saleor-social-auth-0.5.0/saleor_social_auth.egg-info/SOURCES.txt
--rw-r--r--   0 ace        (502) staff       (20)        1 2022-10-19 07:57:51.000000 saleor-social-auth-0.5.0/saleor_social_auth.egg-info/dependency_links.txt
--rw-r--r--   0 ace        (502) staff       (20)       67 2022-10-19 07:57:51.000000 saleor-social-auth-0.5.0/saleor_social_auth.egg-info/entry_points.txt
--rw-r--r--   0 ace        (502) staff       (20)      184 2022-10-19 07:57:51.000000 saleor-social-auth-0.5.0/saleor_social_auth.egg-info/requires.txt
--rw-r--r--   0 ace        (502) staff       (20)       12 2022-10-19 07:57:51.000000 saleor-social-auth-0.5.0/saleor_social_auth.egg-info/top_level.txt
--rw-r--r--   0 ace        (502) staff       (20)        1 2021-09-15 04:49:23.000000 saleor-social-auth-0.5.0/saleor_social_auth.egg-info/zip-safe
--rw-r--r--   0 ace        (502) staff       (20)       38 2022-10-19 07:57:51.598983 saleor-social-auth-0.5.0/setup.cfg
--rw-r--r--   0 ace        (502) staff       (20)     1341 2022-10-19 07:38:38.000000 saleor-social-auth-0.5.0/setup.py
-drwxr-xr-x   0 ace        (502) staff       (20)        0 2022-10-19 07:57:51.598145 saleor-social-auth-0.5.0/social_auth/
--rw-r--r--   0 ace        (502) staff       (20)      209 2021-08-23 07:27:45.000000 saleor-social-auth-0.5.0/social_auth/__init__.py
--rw-r--r--   0 ace        (502) staff       (20)     1990 2022-08-26 16:13:17.000000 saleor-social-auth-0.5.0/social_auth/apps.py
--rw-r--r--   0 ace        (502) staff       (20)     9845 2022-10-18 02:13:43.000000 saleor-social-auth-0.5.0/social_auth/plugin.py
--rw-r--r--   0 ace        (502) staff       (20)     1338 2021-08-23 07:27:45.000000 saleor-social-auth-0.5.0/social_auth/strategy.py
--rw-r--r--   0 ace        (502) staff       (20)     4015 2021-08-23 01:31:22.000000 saleor-social-auth-0.5.0/social_auth/utils.py
+drwxr-xr-x   0 ace        (502) staff       (20)        0 2023-05-18 15:55:16.071102 saleor-social-auth-0.6.0/
+-rw-r--r--   0 ace        (502) staff       (20)     1064 2021-08-17 07:53:44.000000 saleor-social-auth-0.6.0/LICENSE
+-rw-r--r--   0 ace        (502) staff       (20)     1911 2023-05-18 15:55:16.070778 saleor-social-auth-0.6.0/PKG-INFO
+-rw-r--r--   0 ace        (502) staff       (20)     1321 2022-02-09 09:02:49.000000 saleor-social-auth-0.6.0/README.md
+-rw-r--r--   0 ace        (502) staff       (20)      231 2021-08-17 07:53:44.000000 saleor-social-auth-0.6.0/pyproject.toml
+drwxr-xr-x   0 ace        (502) staff       (20)        0 2023-05-18 15:55:16.066953 saleor-social-auth-0.6.0/saleor_social_auth.egg-info/
+-rw-r--r--   0 ace        (502) staff       (20)     1911 2023-05-18 15:55:16.000000 saleor-social-auth-0.6.0/saleor_social_auth.egg-info/PKG-INFO
+-rw-r--r--   0 ace        (502) staff       (20)      443 2023-05-18 15:55:16.000000 saleor-social-auth-0.6.0/saleor_social_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 ace        (502) staff       (20)        1 2023-05-18 15:55:16.000000 saleor-social-auth-0.6.0/saleor_social_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 ace        (502) staff       (20)       67 2023-05-18 15:55:16.000000 saleor-social-auth-0.6.0/saleor_social_auth.egg-info/entry_points.txt
+-rw-r--r--   0 ace        (502) staff       (20)      184 2023-05-18 15:55:16.000000 saleor-social-auth-0.6.0/saleor_social_auth.egg-info/requires.txt
+-rw-r--r--   0 ace        (502) staff       (20)       12 2023-05-18 15:55:16.000000 saleor-social-auth-0.6.0/saleor_social_auth.egg-info/top_level.txt
+-rw-r--r--   0 ace        (502) staff       (20)        1 2021-09-15 04:49:23.000000 saleor-social-auth-0.6.0/saleor_social_auth.egg-info/zip-safe
+-rw-r--r--   0 ace        (502) staff       (20)       38 2023-05-18 15:55:16.071221 saleor-social-auth-0.6.0/setup.cfg
+-rw-r--r--   0 ace        (502) staff       (20)     1341 2023-05-18 15:46:30.000000 saleor-social-auth-0.6.0/setup.py
+drwxr-xr-x   0 ace        (502) staff       (20)        0 2023-05-18 15:55:16.069946 saleor-social-auth-0.6.0/social_auth/
+-rw-r--r--   0 ace        (502) staff       (20)      209 2021-08-23 07:27:45.000000 saleor-social-auth-0.6.0/social_auth/__init__.py
+-rw-r--r--   0 ace        (502) staff       (20)     1990 2022-08-26 16:13:17.000000 saleor-social-auth-0.6.0/social_auth/apps.py
+-rw-r--r--   0 ace        (502) staff       (20)    10092 2023-05-18 15:37:22.000000 saleor-social-auth-0.6.0/social_auth/plugin.py
+-rw-r--r--   0 ace        (502) staff       (20)     1336 2023-01-20 08:27:02.000000 saleor-social-auth-0.6.0/social_auth/strategy.py
+-rw-r--r--   0 ace        (502) staff       (20)     4015 2021-08-23 01:31:22.000000 saleor-social-auth-0.6.0/social_auth/utils.py
```

### Comparing `saleor-social-auth-0.5.0/LICENSE` & `saleor-social-auth-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saleor-social-auth-0.5.0/PKG-INFO` & `saleor-social-auth-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saleor-social-auth
-Version: 0.5.0
+Version: 0.6.0
 Summary: Social auth plugin (wx, alipay & etc.) for Saleor
 Home-page: https://github.com/ace-han/social_auth
 Author: Ace Han
 Author-email: ace.jl.han@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `saleor-social-auth-0.5.0/README.md` & `saleor-social-auth-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `saleor-social-auth-0.5.0/saleor_social_auth.egg-info/PKG-INFO` & `saleor-social-auth-0.6.0/saleor_social_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saleor-social-auth
-Version: 0.5.0
+Version: 0.6.0
 Summary: Social auth plugin (wx, alipay & etc.) for Saleor
 Home-page: https://github.com/ace-han/social_auth
 Author: Ace Han
 Author-email: ace.jl.han@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `saleor-social-auth-0.5.0/setup.py` & `saleor-social-auth-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 README = 'file README.md'
 with open("README.md") as readme:
     README = readme.read()
 
 setup(
     name="saleor-social-auth",
-    version="0.5.0",
+    version="0.6.0",
     description="Social auth plugin (wx, alipay & etc.) for Saleor",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/ace-han/social_auth",
     author="Ace Han",
     author_email="ace.jl.han@gmail.com",
     license="MIT",
```

### Comparing `saleor-social-auth-0.5.0/social_auth/apps.py` & `saleor-social-auth-0.6.0/social_auth/apps.py`

 * *Files identical despite different names*

### Comparing `saleor-social-auth-0.5.0/social_auth/plugin.py` & `saleor-social-auth-0.6.0/social_auth/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,26 +219,35 @@
         # although in the frontend it's `refreshToken` graphene will transform to `refresh_token`
         # `saleor-dashboard/src/auth/hooks/useExternalAuthProvider.ts`
         # const token = getTokens().refresh;
         # const input = JSON.stringify({
         #   refreshToken: token
         # });
         # return tokenRefresh({ variables: { input, pluginId: authPlugin } }).then(...)
-        refresh_token_code = 'refresh_token'
+        # refresh_token_code = 'refresh_token'
+
+        # by debug, it's `refreshToken` instead of `refresh_token`
+        refresh_token_code = 'refreshToken'
         refresh_token = data.get(refresh_token_code) or refresh_token
         payload = RefreshToken.clean_refresh_token(refresh_token)
 
         # None when we got refresh_token from cookie.
+        csrf_token = None
         if not data.get(refresh_token_code):
             csrf_token = data.get(refresh_token_code)
             RefreshToken.clean_csrf_token(csrf_token, payload)
 
         user = RefreshToken.get_user(payload)
         token = create_access_token(user)
-        return RefreshToken(errors=[], user=user, token=token)
+        return ExternalAccessTokens(
+            token=token,
+            refresh_token=refresh_token,
+            csrf_token=csrf_token,
+            user=user
+        )
 
     def external_verify(
         self, data: dict, request: WSGIRequest, previous_value
     ) -> Tuple[Optional["User"], dict]:
         # utilize existing code
         payload = VerifyToken.get_payload(data['token'])
         user = VerifyToken.get_user(payload)
```

### Comparing `saleor-social-auth-0.5.0/social_auth/strategy.py` & `saleor-social-auth-0.6.0/social_auth/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.shortcuts import resolve_url
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.functional import Promise
 from social_django.strategy import DjangoStrategy
 
 class SaleorPluginStrategy(DjangoStrategy):
 
     def __init__(self, storage, settings, request_data, *args, **kwargs):
         # loading settings from dashboard admin
@@ -13,15 +13,15 @@
 
     def get_setting(self, name):
         # copy from social_django.strategy.DjangoStrategy
         value = self.settings[name]
         # Force text on URL named settings that are instance of Promise
         if name.endswith('_URL'):
             if isinstance(value, Promise):
-                value = force_text(value)
+                value = force_str(value)
             value = resolve_url(value)
         return value
 
     def request_data(self, merge=True):
         # graphql may not include query_string or data in request directly
         return self.req_data
```

### Comparing `saleor-social-auth-0.5.0/social_auth/utils.py` & `saleor-social-auth-0.6.0/social_auth/utils.py`

 * *Files identical despite different names*

