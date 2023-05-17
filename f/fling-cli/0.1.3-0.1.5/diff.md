# Comparing `tmp/fling_cli-0.1.3.tar.gz` & `tmp/fling_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_cli-0.1.3.tar", max compression
+gzip compressed data, was "fling_cli-0.1.5.tar", max compression
```

## Comparing `fling_cli-0.1.3.tar` & `fling_cli-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2163 2023-04-05 23:25:42.977524 fling_cli-0.1.3/README.md
--rw-r--r--   0        0        0       22 2023-04-27 22:06:05.211556 fling_cli-0.1.3/fling_cli/__init__.py
--rw-r--r--   0        0        0     2040 2023-04-13 01:15:50.829929 fling_cli-0.1.3/fling_cli/auth.py
--rw-r--r--   0        0        0        0 2023-04-04 19:06:55.600802 fling_cli-0.1.3/fling_cli/bin/__init__.py
--rw-r--r--   0        0        0     6849 2023-04-27 22:05:56.105344 fling_cli-0.1.3/fling_cli/bin/fling.py
--rw-r--r--   0        0        0     3834 2023-04-08 02:13:26.640377 fling_cli-0.1.3/fling_cli/logo-hc.txt
--rw-r--r--   0        0        0      861 2023-04-27 22:06:13.497372 fling_cli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 fling_cli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2163 2023-04-05 23:25:42.977524 fling_cli-0.1.5/README.md
+-rw-r--r--   0        0        0      647 2023-05-17 22:43:54.774155 fling_cli-0.1.5/fling_cli/__init__.py
+-rw-r--r--   0        0        0     2190 2023-05-17 22:30:05.611005 fling_cli-0.1.5/fling_cli/auth.py
+-rw-r--r--   0        0        0        0 2023-04-04 19:06:55.600802 fling_cli-0.1.5/fling_cli/bin/__init__.py
+-rw-r--r--   0        0        0     6306 2023-05-13 22:09:25.053951 fling_cli-0.1.5/fling_cli/bin/fling.py
+-rw-r--r--   0        0        0     1492 2023-05-13 23:40:28.872299 fling_cli-0.1.5/fling_cli/certbot_fling_plugin.py
+-rw-r--r--   0        0        0     3834 2023-04-08 02:13:26.640377 fling_cli-0.1.5/fling_cli/logo-hc.txt
+-rw-r--r--   0        0        0      990 2023-05-17 22:43:43.996942 fling_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 fling_cli-0.1.5/PKG-INFO
```

### Comparing `fling_cli-0.1.3/README.md` & `fling_cli-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.3/fling_cli/auth.py` & `fling_cli-0.1.5/fling_cli/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 import random
 import signal
 import string
 from subprocess import call
 
 import keyring
 import uvicorn
@@ -29,14 +30,17 @@
     @app.get("/callback")
     async def callback(state: str, token: str, username: str):
         # Die after this request finishes, no matter what
 
         if state != stored_state:
             raise Exception("State doesn't match, bad!")
         print(f"Saving token for `{username}` to keyring.")
+        os.makedirs("~/.flingdev", exist_ok=True)
+        with open("flinguser.txt", "w") as userfile:
+            userfile.write(username)
         keyring.set_password("fling-github-token", username, token)
         # default_password = keyring.get_password("fling-github-token", "system-default")
         # if not default_password:
         #     print(f"No default account, Saving token for `{username}` as default.")
         keyring.set_password("fling-github-token", "system-default", token)
         return RedirectResponse('http://localhost:5817', status_code=302)
```

### Comparing `fling_cli-0.1.3/fling_cli/bin/fling.py` & `fling_cli-0.1.5/fling_cli/bin/fling.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,51 +2,34 @@
 # -*- coding: utf-8 -*-
 """Fling CLI commands
 """
 import hashlib
 from pathlib import Path
 import pathlib
 from fling_cli.auth import gh_authenticate
-import keyring
+from fling_cli import get_fling_client
 import rich_click as click
 from click.exceptions import UsageError
 from rich import print, print_json
 from rich.tree import Tree
 from cookiecutter.main import cookiecutter
-from fling_client.client import Client
 from fling_client.api.names import generate_names_namer_get
 from fling_client.api.data import (
     add_data_fling_id_add_post,
     read_data_fling_id_get,
     get_repo_list_repolist_get,
     add_to_index_index_put,
     read_index_index_get,
 )
 from rich.table import Table
-from fling_core import settings
 import gitinfo
 from git import Repo
 from giturlparse import parse
 
 
-def get_fling_client(require_auth=False):
-    username = "system-default"
-    token = keyring.get_password("fling-github-token", username)
-    if not token and require_auth:
-        raise UsageError("No token found, please run ```fling auth``` first.")
-    headers = {"gh-token": token or "none"}
-    fling_client = Client(
-        settings.api_server,
-        headers=headers,
-        verify_ssl=False,
-        timeout=60,
-        raise_on_unexpected_status=True,
-    )
-    return fling_client
-
 
 click.rich_click.USE_RICH_MARKUP = True
 click.rich_click.COMMAND_GROUPS = {
     "fling": [
         {
             "name": "Commands for starting new projects",
             "commands": ["auth", "search", "init", "acknowledge"],
```

### Comparing `fling_cli-0.1.3/fling_cli/logo-hc.txt` & `fling_cli-0.1.5/fling_cli/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.3/pyproject.toml` & `fling_cli-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 [tool.poetry]
 name = "fling-cli"
-version = "0.1.3"
+version = "0.1.5"
 description = "Side Project Management from the command line"
 authors = ["Joshua McKenty <jmckenty@gmail.com>", "Anouk Ruhaak <anoukruhaak@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fling_cli"}]
 
 [tool.poetry.dependencies]
 click = "*"
 python-dotenv = "*"
 cookiecutter = "*"
 rich-click = "*"
 python = "^3.9"
 # fling-client = {path="../fling-client", develop=true}
 # fling-core = {path="../fling-core", develop=true}
-fling-client = "*"
+fling-client = "^0.1.3"
 fling-core = "*"
 keyring = "^23.13.1"
 requests-oauthlib = "^1.3.1"
 uvicorn = "^0.21.1"
 fastapi = "^0.95.0"
 python-git-info = "^0.8.2"
 gitpython = "^3.1.31"
 giturlparse = "^0.10.0"
+certbot = "*"
 
 [tool.poetry.scripts]
 fling = "fling_cli.bin.fling:main"
 git-fling = "fling_cli.bin.fling:main"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.plugins."certbot.plugins"]
+fling_authenticator = "fling_cli.certbot_fling_plugin:Authenticator"
```

### Comparing `fling_cli-0.1.3/PKG-INFO` & `fling_cli-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: fling-cli
-Version: 0.1.3
+Version: 0.1.5
 Summary: Side Project Management from the command line
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: certbot
 Requires-Dist: click
 Requires-Dist: cookiecutter
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
-Requires-Dist: fling-client
+Requires-Dist: fling-client (>=0.1.3,<0.2.0)
 Requires-Dist: fling-core
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: giturlparse (>=0.10.0,<0.11.0)
 Requires-Dist: keyring (>=23.13.1,<24.0.0)
 Requires-Dist: python-dotenv
 Requires-Dist: python-git-info (>=0.8.2,<0.9.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
```

