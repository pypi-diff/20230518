# Comparing `tmp/requests_oidc-0.6.0.tar.gz` & `tmp/requests_oidc-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_oidc-0.6.0.tar", max compression
+gzip compressed data, was "requests_oidc-0.6.1.tar", max compression
```

## Comparing `requests_oidc-0.6.0.tar` & `requests_oidc-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1054 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/LICENSE
--rw-r--r--   0        0        0     3079 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/README.rst
--rw-r--r--   0        0        0      890 2023-05-12 14:40:39.399026 requests_oidc-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      399 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/__main__.py
--rw-r--r--   0        0        0     3292 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/cli.py
--rw-r--r--   0        0        0       41 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/flows/__init__.py
--rw-r--r--   0        0        0     3285 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/flows/auth_code.py
--rw-r--r--   0        0        0     1174 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/flows/client_credentials.py
--rw-r--r--   0        0        0     4021 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/flows/device_code.py
--rw-r--r--   0        0        0     1192 2023-05-12 14:40:01.115653 requests_oidc-0.6.0/src/requests_oidc/flows/token.py
--rw-r--r--   0        0        0      558 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/flows/utils.py
--rw-r--r--   0        0        0     1402 2023-05-12 14:39:40.251995 requests_oidc-0.6.0/src/requests_oidc/plugins.py
--rw-r--r--   0        0        0      170 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/types.py
--rw-r--r--   0        0        0      104 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/utils/__init__.py
--rw-r--r--   0        0        0      930 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/utils/catcher.py
--rw-r--r--   0        0        0      637 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/utils/discovery.py
--rw-r--r--   0        0        0      220 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/utils/scope.py
--rw-r--r--   0        0        0     4099 1970-01-01 00:00:00.000000 requests_oidc-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3500 2023-05-12 18:03:15.200671 requests_oidc-0.6.1/README.rst
+-rw-r--r--   0        0        0      890 2023-05-18 19:44:22.977415 requests_oidc-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      443 2023-05-12 18:04:27.323513 requests_oidc-0.6.1/src/requests_oidc/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/__main__.py
+-rw-r--r--   0        0        0     3292 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/cli.py
+-rw-r--r--   0        0        0       41 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/flows/__init__.py
+-rw-r--r--   0        0        0     3285 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/flows/auth_code.py
+-rw-r--r--   0        0        0     1174 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/flows/client_credentials.py
+-rw-r--r--   0        0        0     4021 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/flows/device_code.py
+-rw-r--r--   0        0        0     1192 2023-05-12 14:40:01.115653 requests_oidc-0.6.1/src/requests_oidc/flows/token.py
+-rw-r--r--   0        0        0      582 2023-05-18 19:43:58.577780 requests_oidc-0.6.1/src/requests_oidc/flows/utils.py
+-rw-r--r--   0        0        0     1372 2023-05-18 19:43:58.581780 requests_oidc-0.6.1/src/requests_oidc/plugins.py
+-rw-r--r--   0        0        0      170 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/types.py
+-rw-r--r--   0        0        0      104 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/utils/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/utils/catcher.py
+-rw-r--r--   0        0        0      637 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/utils/discovery.py
+-rw-r--r--   0        0        0      220 2023-05-12 13:41:52.727655 requests_oidc-0.6.1/src/requests_oidc/utils/scope.py
+-rw-r--r--   0        0        0     4520 1970-01-01 00:00:00.000000 requests_oidc-0.6.1/PKG-INFO
```

### Comparing `requests_oidc-0.6.0/LICENSE` & `requests_oidc-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.0/pyproject.toml` & `requests_oidc-0.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "requests-oidc"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["Tristan Sweeney <tsweeney@dustidentity.com>"]
 readme = "README.rst"
 packages = [{include = "requests_oidc", from = "src"}]
 repository = "https://github.com/tsweeney-dust/requests-oidc"
 documentation = "https://requests-oidc.readthedocs.io/en/latest/"
 license = "MIT"
@@ -25,13 +25,13 @@
 
 
 [tool.poetry.group.dev.dependencies]
 sphinx = ">=5.0.0"
 sphinx-toolbox = "^3.2.0"
 sphinx-copybutton = "^0.5.1"
 types-requests = "^2.28.11.15"
-mypy = "^1.1.1"
+mypy = "^1.3.0"
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `requests_oidc-0.6.0/src/requests_oidc/cli.py` & `requests_oidc-0.6.1/src/requests_oidc/cli.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.0/src/requests_oidc/flows/auth_code.py` & `requests_oidc-0.6.1/src/requests_oidc/flows/auth_code.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.0/src/requests_oidc/flows/client_credentials.py` & `requests_oidc-0.6.1/src/requests_oidc/flows/client_credentials.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.0/src/requests_oidc/flows/device_code.py` & `requests_oidc-0.6.1/src/requests_oidc/flows/device_code.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.0/src/requests_oidc/flows/token.py` & `requests_oidc-0.6.1/src/requests_oidc/flows/token.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.0/src/requests_oidc/flows/utils.py` & `requests_oidc-0.6.1/src/requests_oidc/flows/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from typing import List
 
 
 def access_expired(token: dict, margin: int = 0) -> bool:
     return (time.time()) > token["expires_at"] + margin
 
 
 def refresh_expired(token: dict, margin: int = 0) -> bool:
@@ -10,9 +11,9 @@
         return False
 
     refresh_expires_at = (
         token["refresh_expires_in"] - token["expires_in"] + token["expires_at"]
     )
     return (time.time() + margin) > (refresh_expires_at + margin)
 
-def scope_mismatch(token: dict, scopes: list[str]) -> bool:
+def scope_mismatch(token: dict, scopes: List[str]) -> bool:
     return any(scope not in token['scope'] for scope in scopes)
```

### Comparing `requests_oidc-0.6.0/src/requests_oidc/plugins.py` & `requests_oidc-0.6.1/src/requests_oidc/plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 import json
 import appdirs
 from typing import Optional
 
 
 class PathPlugin:
-    """Same as ``make_oidc_session``, but saves/loads token to OS path."""
+    """Plugin to load / store files to an OS path location"""
 
     def __init__(self, path: Path, *, noload: bool = False, nostore: bool = False) -> None:
         self.path = path
         self.noload = noload
         self.nostore = nostore
 
     def load(self) -> Optional[dict]:
@@ -27,21 +27,21 @@
             return
         
         with self.path.open("w") as f:
             json.dump(token, f)
 
 
 class OSCachedPlugin(PathPlugin):
-    """Same as ``make_oidc_session``, but saves/loads token to the OS-relevant user cache directory (appdata, ~/.cache/..., etc)."""
+    """Same as ``PathPlugin``, but saves/loads to the OS's user-cache directory (appdata, ~/.cache/..., etc)."""
 
     def __init__(
         self,
         appname: str,
         appauthor: str,
-        version: str | None = None,
+        version: Optional[str] = None,
         filename: str = "token.json",
         *, noload: bool = False, nostore: bool = False
     ) -> None:
         dirs = appdirs.AppDirs(appname=appname, appauthor=appauthor, version=version)
         dir = Path(dirs.user_cache_dir)
         dir.mkdir(parents=True, exist_ok=True)
         super().__init__(dir / filename, noload=noload, nostore=nostore)
```

### Comparing `requests_oidc-0.6.0/src/requests_oidc/utils/catcher.py` & `requests_oidc-0.6.1/src/requests_oidc/utils/catcher.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.0/src/requests_oidc/utils/discovery.py` & `requests_oidc-0.6.1/src/requests_oidc/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.6.0/PKG-INFO` & `requests_oidc-0.6.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-oidc
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Home-page: https://github.com/tsweeney-dust/requests-oidc
 License: MIT
 Author: Tristan Sweeney
 Author-email: tsweeney@dustidentity.com
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 3 - Alpha
@@ -25,21 +25,37 @@
 Description-Content-Type: text/x-rst
 
 Requests-OIDC
 =================
 
 .. inclusion-marker-do-not-remove
 
-Implements a simple single-function API for creating a requests ``Session`` that
+Implements a simple API for creating a requests ``Session`` that
 manages your OIDC-discovered OAuth2 session for you.
 
 ::
 
    pip install requests-oidc
 
+.. code-block:: python
+
+   from requests_oidc import make_auth_code_session
+   from requests_oidc.plugins import OSCachedPlugin
+
+   oidc_url = "https://your-oidc-provider.com/.well-known/openid-configuration"
+   client_id = "your-app"
+   port = 8675
+   scope = ["openid", "email", "profile"]
+
+   plugin = OSCachedPlugin("your-app", "your-company")
+
+
+
+   session = make_auth_code_session(oidc_url, client_id, port, scope, plugin=plugin)
+
 
 .. list-table::
 
    * - Package
      - |pypi| |license| |py status| |formats| |python| |py impls| |downloads|
    * - build
      - |checks| |rtd build| |coverage|
```

