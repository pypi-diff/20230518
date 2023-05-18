# Comparing `tmp/postodon-0.0.3.tar.gz` & `tmp/postodon-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postodon-0.0.3.tar", max compression
+gzip compressed data, was "postodon-0.0.4.tar", max compression
```

## Comparing `postodon-0.0.3.tar` & `postodon-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11339 2023-05-15 11:12:33.601442 postodon-0.0.3/LICENSE
--rw-r--r--   0        0        0     2193 2023-05-15 11:12:33.601442 postodon-0.0.3/README.md
--rw-r--r--   0        0        0     1057 2023-05-15 11:12:33.601442 postodon-0.0.3/postodon/__init__.py
--rw-r--r--   0        0        0      294 2023-05-15 11:12:33.601442 postodon-0.0.3/postodon/append_post.py
--rw-r--r--   0        0        0     1611 2023-05-15 11:12:33.601442 postodon-0.0.3/postodon/select_post.py
--rw-r--r--   0        0        0      520 2023-05-15 11:12:33.601442 postodon-0.0.3/postodon/submit_post.py
--rw-r--r--   0        0        0      345 2023-05-15 11:12:33.601442 postodon-0.0.3/postodon/utils.py
--rw-r--r--   0        0        0     1019 2023-05-15 11:12:33.601442 postodon-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 postodon-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-05-18 10:45:27.061974 postodon-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2527 2023-05-18 10:45:27.061974 postodon-0.0.4/README.md
+-rw-r--r--   0        0        0     1057 2023-05-18 10:45:27.061974 postodon-0.0.4/postodon/__init__.py
+-rw-r--r--   0        0        0      294 2023-05-18 10:45:27.061974 postodon-0.0.4/postodon/append_post.py
+-rw-r--r--   0        0        0     1611 2023-05-18 10:45:27.061974 postodon-0.0.4/postodon/select_post.py
+-rw-r--r--   0        0        0      520 2023-05-18 10:45:27.061974 postodon-0.0.4/postodon/submit_post.py
+-rw-r--r--   0        0        0      345 2023-05-18 10:45:27.061974 postodon-0.0.4/postodon/utils.py
+-rw-r--r--   0        0        0     1127 2023-05-18 10:45:27.061974 postodon-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 postodon-0.0.4/PKG-INFO
```

### Comparing `postodon-0.0.3/LICENSE` & `postodon-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `postodon-0.0.3/README.md` & `postodon-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 # postodon
 
 [![PyPI](https://img.shields.io/pypi/v/postodon.svg)](https://pypi.org/project/postodon/)
 [![Changelog](https://img.shields.io/github/v/release/msleigh/postodon?include_prereleases&label=changelog)](https://github.com/msleigh/postodon/releases)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/msleigh/postodon/blob/main/LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
-Randomly posts things to Mastadon from a list using the API.
+Randomly posts things to Mastadon from a pre-defined list, using the Mastodon API.
 
 The list of posts is a JSON file:
 
     [
         {"content": "Text of the post", "id": 1, "status": "unposted"},
         ...,
     ]
 
 The command `postodon` randomly selects an unposted post, posts it to Mastodon, and marks it as posted in the list. If there are no unposted items, an already-posted item is used instead.
 
+## Requirements
+
+FLAFL requires Python 3.7+. It is tested on Linux and macOS.
+
 ## Installation
 
-Install:
+Postodon is published as a Python package and can be installed with `pip`, ideally by using a virtual environment. Open up a terminal and install with:
 
-    python3 -m venv .venv
-    source .venv/bin/activate
     pip install postodon
 
-## Usage
-
-### Setup
+## Configuration
 
  - Register an application as described here: https://docs.joinmastodon.org/client/token/#app
  - Get an access token as described here: https://docs.joinmastodon.org/client/authorized/#flow
  - Securely store the returned `access_token` for future reference
- - Edit `config.json` to include the name of the Mastodon instance and the name of the posts file, e.g. `posts.json`
-
-### Use
+ - Edit `config.json` to include the name of the Mastodon instance and the name of the posts file, e.g. `posts.json` - Put the access token in an environment variable called `AUTH_TOKEN`
 
-To use, put the access token in an environment variable called `AUTH_TOKEN`:
+      export AUTH_TOKEN=<your_access_token_here>
 
-    export AUTH_TOKEN=<your_access_token_here>
+## Usage
 
-To publicly post a random post, marked as English, and update the list (mark the post having been posted):
+To publicly post a random post from the list (marked as English), and update the list (i.e. mark the post having been posted):
 
     postodon
 
-(This is a shortcut for `postodon post`). NB if there are no unposted posts left in the list, this will return a random post from the 'posted' selection.
+This is a shortcut for `postodon post`. NB if there are no unposted items left in the list, a randomly-selected item from the 'posted' selection will be posted instead.
 
-To select a random post from the list without either updating the list or posting (dry-run mode):
+To randomly select an item from the list without either updating the list or posting (dry-run mode):
 
     postodon post -n
 
 To add new posts to the list for future posting:
 
     postodon add "Text of post"
```

### Comparing `postodon-0.0.3/postodon/__init__.py` & `postodon-0.0.4/postodon/__init__.py`

 * *Files identical despite different names*

### Comparing `postodon-0.0.3/postodon/select_post.py` & `postodon-0.0.4/postodon/select_post.py`

 * *Files identical despite different names*

### Comparing `postodon-0.0.3/postodon/submit_post.py` & `postodon-0.0.4/postodon/submit_post.py`

 * *Files identical despite different names*

### Comparing `postodon-0.0.3/pyproject.toml` & `postodon-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "postodon"
-version = "0.0.3"
+version = "0.0.4"
 description = "Post to Mastodon"
-authors = ["msleigh"]
+authors = ["msleigh <msleigh@noreply.users.github.com>"]
+license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "postodon"}]
-license = "Apache-2.0"
 classifiers = [
     "Development Status :: 1 - Planning",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
@@ -26,14 +26,18 @@
 sphinx = "^7.0.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1.12"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
+black = "^23.3.0"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
 
-[tool.project.scripts]
+[tool.poetry.scripts]
 postodon = "postodon:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `postodon-0.0.3/PKG-INFO` & `postodon-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: postodon
-Version: 0.0.3
+Version: 0.0.4
 Summary: Post to Mastodon
 Home-page: https://github.com/msleigh/postodon
 License: Apache-2.0
 Author: msleigh
+Author-email: msleigh@noreply.users.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -24,56 +25,55 @@
 Description-Content-Type: text/markdown
 
 # postodon
 
 [![PyPI](https://img.shields.io/pypi/v/postodon.svg)](https://pypi.org/project/postodon/)
 [![Changelog](https://img.shields.io/github/v/release/msleigh/postodon?include_prereleases&label=changelog)](https://github.com/msleigh/postodon/releases)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/msleigh/postodon/blob/main/LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
-Randomly posts things to Mastadon from a list using the API.
+Randomly posts things to Mastadon from a pre-defined list, using the Mastodon API.
 
 The list of posts is a JSON file:
 
     [
         {"content": "Text of the post", "id": 1, "status": "unposted"},
         ...,
     ]
 
 The command `postodon` randomly selects an unposted post, posts it to Mastodon, and marks it as posted in the list. If there are no unposted items, an already-posted item is used instead.
 
+## Requirements
+
+FLAFL requires Python 3.7+. It is tested on Linux and macOS.
+
 ## Installation
 
-Install:
+Postodon is published as a Python package and can be installed with `pip`, ideally by using a virtual environment. Open up a terminal and install with:
 
-    python3 -m venv .venv
-    source .venv/bin/activate
     pip install postodon
 
-## Usage
-
-### Setup
+## Configuration
 
  - Register an application as described here: https://docs.joinmastodon.org/client/token/#app
  - Get an access token as described here: https://docs.joinmastodon.org/client/authorized/#flow
  - Securely store the returned `access_token` for future reference
- - Edit `config.json` to include the name of the Mastodon instance and the name of the posts file, e.g. `posts.json`
-
-### Use
+ - Edit `config.json` to include the name of the Mastodon instance and the name of the posts file, e.g. `posts.json` - Put the access token in an environment variable called `AUTH_TOKEN`
 
-To use, put the access token in an environment variable called `AUTH_TOKEN`:
+      export AUTH_TOKEN=<your_access_token_here>
 
-    export AUTH_TOKEN=<your_access_token_here>
+## Usage
 
-To publicly post a random post, marked as English, and update the list (mark the post having been posted):
+To publicly post a random post from the list (marked as English), and update the list (i.e. mark the post having been posted):
 
     postodon
 
-(This is a shortcut for `postodon post`). NB if there are no unposted posts left in the list, this will return a random post from the 'posted' selection.
+This is a shortcut for `postodon post`. NB if there are no unposted items left in the list, a randomly-selected item from the 'posted' selection will be posted instead.
 
-To select a random post from the list without either updating the list or posting (dry-run mode):
+To randomly select an item from the list without either updating the list or posting (dry-run mode):
 
     postodon post -n
 
 To add new posts to the list for future posting:
 
     postodon add "Text of post"
```

