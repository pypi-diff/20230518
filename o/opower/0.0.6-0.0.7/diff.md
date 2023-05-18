# Comparing `tmp/opower-0.0.6.tar.gz` & `tmp/opower-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opower-0.0.6.tar", last modified: Fri May 12 02:18:42 2023, max compression
+gzip compressed data, was "opower-0.0.7.tar", last modified: Thu May 18 18:10:38 2023, max compression
```

## Comparing `opower-0.0.6.tar` & `opower-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:18:42.964003 opower-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 02:18:27.000000 opower-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-12 02:18:42.964003 opower-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-12 02:18:27.000000 opower-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-12 02:18:27.000000 opower-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-12 02:18:42.964003 opower-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:18:42.956003 opower-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-12 02:18:27.000000 opower-0.0.6/src/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:18:42.960003 opower-0.0.6/src/opower/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-12 02:18:27.000000 opower-0.0.6/src/opower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14305 2023-05-12 02:18:27.000000 opower-0.0.6/src/opower/opower.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:18:42.964003 opower-0.0.6/src/opower/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-12 02:18:27.000000 opower-0.0.6/src/opower/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-12 02:18:27.000000 opower-0.0.6/src/opower/utilities/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-12 02:18:27.000000 opower-0.0.6/src/opower/utilities/pge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:18:42.960003 opower-0.0.6/src/opower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-12 02:18:42.000000 opower-0.0.6/src/opower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-12 02:18:42.000000 opower-0.0.6/src/opower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:18:42.000000 opower-0.0.6/src/opower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 02:18:42.000000 opower-0.0.6/src/opower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 02:18:42.000000 opower-0.0.6/src/opower.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:18:42.964003 opower-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-12 02:18:27.000000 opower-0.0.6/tests/test_opower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.479838 opower-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 18:10:19.000000 opower-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-18 18:10:38.479838 opower-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-18 18:10:19.000000 opower-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-18 18:10:19.000000 opower-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-18 18:10:38.479838 opower-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.475838 opower-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-18 18:10:19.000000 opower-0.0.7/src/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.475838 opower-0.0.7/src/opower/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/opower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.479838 opower-0.0.7/src/opower/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/utilities/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/utilities/pge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/utilities/pse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.479838 opower-0.0.7/src/opower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-18 18:10:38.000000 opower-0.0.7/src/opower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-18 18:10:38.000000 opower-0.0.7/src/opower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:10:38.000000 opower-0.0.7/src/opower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 18:10:38.000000 opower-0.0.7/src/opower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 18:10:38.000000 opower-0.0.7/src/opower.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.479838 opower-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-18 18:10:19.000000 opower-0.0.7/tests/test_opower.py
```

### Comparing `opower-0.0.6/LICENSE` & `opower-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opower-0.0.6/PKG-INFO` & `opower-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `opower-0.0.6/README.md` & `opower-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `opower-0.0.6/pyproject.toml` & `opower-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "opower"
-version = "0.0.6"
+version = "0.0.7"
 license = {text = "Apache-2.0"}
 authors = [
     { name="tronikos", email="tronikos@gmail.com" },
 ]
 description = "A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `opower-0.0.6/src/demo.py` & `opower-0.0.7/src/demo.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.6/src/opower/__init__.py` & `opower-0.0.7/src/opower/__init__.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.6/src/opower/opower.py` & `opower-0.0.7/src/opower/opower.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,16 @@
         self.username = username
         self.password = password
         self.customer = None
 
     async def async_login(self) -> None:
         """Login to the utility website and authorize opower.com for access."""
         url = await self.utility.login(self.session, self.username, self.password)
-        await self._async_authorize(url)
+        if url is not None:
+            await self._async_authorize(url)
 
     async def _async_authorize(self, url: str) -> None:
         # Fetch the URL on the utility website to get RelayState and SAMLResponse.
         async with self.session.get(url) as resp:
             result = await resp.text()
         action_url, hidden_inputs = _get_form_action_url_and_hidden_inputs(result)
         assert action_url == "https://sso2.opower.com/sp/ACS.saml2"
```

### Comparing `opower-0.0.6/src/opower/utilities/base.py` & `opower-0.0.7/src/opower/utilities/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,13 +31,16 @@
         Should match the siteTimeZoneId of the API responses.
         """
         raise NotImplementedError
 
     @staticmethod
     async def login(
         session: aiohttp.ClientSession, username: str, password: str
-    ) -> str:
-        """Login to the utility website and return a URL where we can authorize opower.com.
+    ) -> str | None:
+        """Login to the utility website.
+
+        Returns either a URL for SAML authentication with opower.com,
+        or directly handles authentication and returns None.
 
         Any failure to login should raise ClientResponseError with status 401 or 403.
         """
         raise NotImplementedError
```

### Comparing `opower-0.0.6/src/opower/utilities/pge.py` & `opower-0.0.7/src/opower/utilities/pge.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.6/src/opower.egg-info/PKG-INFO` & `opower-0.0.7/src/opower.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

