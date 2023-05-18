# Comparing `tmp/imessagedb-1.2.5.tar.gz` & `tmp/imessagedb-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.2.5.tar", max compression
+gzip compressed data, was "imessagedb-1.2.6.tar", max compression
```

## Comparing `imessagedb-1.2.5.tar` & `imessagedb-1.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1070 2023-05-18 01:13:42.193124 imessagedb-1.2.5/LICENSE
--rw-r--r--   0        0        0     8458 2023-05-18 01:13:42.193124 imessagedb-1.2.5/README.md
--rw-r--r--   0        0        0     1256 2023-05-18 01:14:18.025756 imessagedb-1.2.5/pyproject.toml
--rw-r--r--   0        0        0    10022 2023-05-18 01:13:42.197124 imessagedb-1.2.5/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-18 01:13:42.197124 imessagedb-1.2.5/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8456 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3049 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2133 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/chat.py
--rw-r--r--   0        0        0     2510 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3301 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/default.ini
--rw-r--r--   0        0        0      985 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/handle.py
--rw-r--r--   0        0        0     1640 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/handles.py
--rw-r--r--   0        0        0    23073 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/html.py
--rw-r--r--   0        0        0     5138 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/message.py
--rw-r--r--   0        0        0     5359 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/messages.py
--rw-r--r--   0        0        0     4182 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/text.py
--rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 imessagedb-1.2.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-05-18 01:55:28.519982 imessagedb-1.2.6/LICENSE
+-rw-r--r--   0        0        0     8458 2023-05-18 01:55:28.519982 imessagedb-1.2.6/README.md
+-rw-r--r--   0        0        0     1309 2023-05-18 01:56:15.252258 imessagedb-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0    10222 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8456 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3049 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2133 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     2510 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3301 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/default.ini
+-rw-r--r--   0        0        0      985 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     1640 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/handles.py
+-rw-r--r--   0        0        0    23073 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/html.py
+-rw-r--r--   0        0        0     5138 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/message.py
+-rw-r--r--   0        0        0     5359 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/messages.py
+-rw-r--r--   0        0        0     4182 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/text.py
+-rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 imessagedb-1.2.6/PKG-INFO
```

### Comparing `imessagedb-1.2.5/LICENSE` & `imessagedb-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/README.md` & `imessagedb-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/pyproject.toml` & `imessagedb-1.2.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imessagedb"
-version = "1.2.5"
+version = "1.2.6"
 description = "Reads and displays the Apple iMessage database"
 authors = ["xev <git@schore.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -18,14 +18,17 @@
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 myst-nb = {version = "^0.17.2", python = "^3.9"}
 sphinx-autoapi = "^2.1.0"
 sphinx-rtd-theme = "^1.2.0"
 python-semantic-release = "^7.33.4"
 
+[tool.poetry.scripts]
+imessagedb = 'imessagedb:run'
+
 [tool.semantic_release]
 version_variable = "pyproject.toml:version"
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
 build_command = "poetry build"              # build dists
 dist_path = "dist/"                         # where to put dists
 upload_to_release = true                    # auto-create GitHub release
```

### Comparing `imessagedb-1.2.5/src/imessagedb/__init__.py` & `imessagedb-1.2.6/src/imessagedb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-provides access to the iMessage chat.db, including parsing and output
+Provides access to the iMessage chat.db, including parsing and output
 
 """
 from importlib.metadata import version
 
 # read version from installed package
 
 __version__ = version("imessagedb")
@@ -149,15 +149,15 @@
         result[key] = number_list
     return result
 
 
 def run() -> None:
     logging.basicConfig(level=logging.INFO, format='%(asctime)s <%(name)s> %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
     logger = logging.getLogger('main')
-    logger.info("Processing parameters")
+    logger.debug("Processing parameters")
 
     argument_parser = argparse.ArgumentParser()
     person_mutex_group = argument_parser.add_mutually_exclusive_group()
     person_mutex_group.add_argument('--handle', help="A list of handles to search against", nargs='*')
     person_mutex_group.add_argument("--name", help="Person to get conversations about")
     argument_parser.add_argument("-c", "--configfile", help="Location of the configuration file",
                                  default=f'{os.environ["HOME"]}/.config/iMessageDB.ini')
@@ -171,17 +171,22 @@
     copy_mutex_group = argument_parser.add_mutually_exclusive_group()
     copy_mutex_group.add_argument("-f", "--force", help="Force a copy of the attachments", action="store_true")
     copy_mutex_group.add_argument("--no_copy", help="Don't copy the attachments", action="store_true")
     argument_parser.add_argument("--no_attachments", help="Don't process attachments at all", action="store_true")
     argument_parser.add_argument("-v", "--verbose", help="Turn on additional output", action="store_true")
     argument_parser.add_argument('--start_time', help="The start time of the messages in YYYY-MM-DD HH:MM:SS format")
     argument_parser.add_argument('--end_time', help="The end time of the messages in YYYY-MM-DD HH:MM:SS format")
+    argument_parser.add_argument('--version', help="Prints the version number", action="store_true")
 
     args = argument_parser.parse_args()
 
+    if args.version:
+        print(f"imessagedb {__version__}", file=sys.stderr)
+        exit(0)
+
     # First read in the configuration file, creating it if need be, then overwrite the values from the command line
     if not os.path.exists(args.configfile):
         _create_default_configuration(args.configfile)
     config = configparser.ConfigParser()
     config.read(args.configfile)
 
     CONTROL = 'CONTROL'
```

### Comparing `imessagedb-1.2.5/src/imessagedb/attachment.py` & `imessagedb-1.2.6/src/imessagedb/attachment.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/src/imessagedb/attachments.py` & `imessagedb-1.2.6/src/imessagedb/attachments.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/src/imessagedb/chat.py` & `imessagedb-1.2.6/src/imessagedb/chat.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/src/imessagedb/chats.py` & `imessagedb-1.2.6/src/imessagedb/chats.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/src/imessagedb/db.py` & `imessagedb-1.2.6/src/imessagedb/db.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/src/imessagedb/default.ini` & `imessagedb-1.2.6/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/src/imessagedb/handle.py` & `imessagedb-1.2.6/src/imessagedb/handle.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/src/imessagedb/handles.py` & `imessagedb-1.2.6/src/imessagedb/handles.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/src/imessagedb/html.py` & `imessagedb-1.2.6/src/imessagedb/html.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/src/imessagedb/message.py` & `imessagedb-1.2.6/src/imessagedb/message.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/src/imessagedb/messages.py` & `imessagedb-1.2.6/src/imessagedb/messages.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/src/imessagedb/text.py` & `imessagedb-1.2.6/src/imessagedb/text.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.5/PKG-INFO` & `imessagedb-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.2.5
+Version: 1.2.6
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

