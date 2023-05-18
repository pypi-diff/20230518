# Comparing `tmp/doing-cli-1.5.2.tar.gz` & `tmp/doing-cli-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doing-cli-1.5.2.tar", last modified: Mon Apr 17 18:40:29 2023, max compression
+gzip compressed data, was "doing-cli-1.5.3.tar", last modified: Thu May 18 07:48:08 2023, max compression
```

## Comparing `doing-cli-1.5.2.tar` & `doing-cli-1.5.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-17 18:39:54.000000 doing-cli-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-17 18:40:29.755096 doing-cli-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-17 18:39:54.000000 doing-cli-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:40:29.755096 doing-cli-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-17 18:39:54.000000 doing-cli-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.751096 doing-cli-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.751096 doing-cli-1.5.2/src/doing/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/init/_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/init/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/issue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/issue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/issue/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/issue/create_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/issue/open_issue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/list/_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/list/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/open/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/open/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/open/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/pr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/pr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/pr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/pr/create_pr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/pr/list_pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/pr/open_pr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing/workon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/workon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-17 18:39:54.000000 doing-cli-1.5.2/src/doing/workon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:40:29.755096 doing-cli-1.5.2/src/doing_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 18:40:29.000000 doing-cli-1.5.2/src/doing_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:48:08.455517 doing-cli-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-18 07:47:19.000000 doing-cli-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-18 07:48:08.455517 doing-cli-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-18 07:47:19.000000 doing-cli-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 07:48:08.455517 doing-cli-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-18 07:47:19.000000 doing-cli-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:48:08.451517 doing-cli-1.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:48:08.451517 doing-cli-1.5.3/src/doing/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:48:08.451517 doing-cli-1.5.3/src/doing/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/init/_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/init/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:48:08.451517 doing-cli-1.5.3/src/doing/issue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/issue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/issue/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/issue/create_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/issue/open_issue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:48:08.455517 doing-cli-1.5.3/src/doing/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/list/_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/list/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:48:08.455517 doing-cli-1.5.3/src/doing/open/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/open/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/open/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:48:08.455517 doing-cli-1.5.3/src/doing/pr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/pr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/pr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/pr/create_pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/pr/list_pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/pr/open_pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:48:08.455517 doing-cli-1.5.3/src/doing/workon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/workon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-18 07:47:19.000000 doing-cli-1.5.3/src/doing/workon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:48:08.455517 doing-cli-1.5.3/src/doing_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-18 07:48:08.000000 doing-cli-1.5.3/src/doing_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-18 07:48:08.000000 doing-cli-1.5.3/src/doing_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 07:48:08.000000 doing-cli-1.5.3/src/doing_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-18 07:48:08.000000 doing-cli-1.5.3/src/doing_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-18 07:48:08.000000 doing-cli-1.5.3/src/doing_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 07:48:08.000000 doing-cli-1.5.3/src/doing_cli.egg-info/top_level.txt
```

### Comparing `doing-cli-1.5.2/LICENSE` & `doing-cli-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/PKG-INFO` & `doing-cli-1.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doing-cli
-Version: 1.5.2
+Version: 1.5.3
 Summary: CLI tool to simplify the development workflow on azure devops
 Home-page: https://github.com/ing-bank/doing-cli
 Author: ING Bank N.V.
 Author-email: tim.vink@ing.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doing-cli-1.5.2/README.md` & `doing-cli-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/setup.py` & `doing-cli-1.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/cli.py` & `doing-cli-1.5.3/src/doing/cli.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/exceptions.py` & `doing-cli-1.5.3/src/doing/exceptions.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/init/_init.py` & `doing-cli-1.5.3/src/doing/init/_init.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/issue/commands.py` & `doing-cli-1.5.3/src/doing/issue/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -107,35 +107,45 @@
     "-s",
     required=False,
     default="",
     type=str,
     help="The number of story points to assign. Not assigned if not specified.",
     show_envvar=True,
 )
+@click.option(
+    "--add-to-current-sprint/--do-not-add-to-current-sprint",
+    required=False,
+    default=False,
+    type=bool,
+    help="If the item needs to be added to the current sprint. Defaults to false",
+    show_envvar=True,
+)
 def create(
     issue: str,
     mine: bool,
     assignee: str,
     body: str,
     type: str,
     label: str,
     parent: str,
     web: bool,
     story_points: str,
+    add_to_current_sprint,
 ) -> None:
     """Create an issue.
 
     ISSUE is the title to be used for the new work item.
     """
     work_item_id = cmd_create_issue(
         title=issue,
         mine=mine,
         assignee=assignee,
         label=label,
         body=body,
         type=type,
         parent=parent,
         story_points=story_points,
+        add_to_current_sprint=add_to_current_sprint,
         **get_common_options(),
     )
     if web:
         cmd_open_issue(work_item_id)
```

### Comparing `doing-cli-1.5.2/src/doing/issue/create_issue.py` & `doing-cli-1.5.3/src/doing/issue/create_issue.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/list/_list.py` & `doing-cli-1.5.3/src/doing/list/_list.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/list/commands.py` & `doing-cli-1.5.3/src/doing/list/commands.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/open/commands.py` & `doing-cli-1.5.3/src/doing/open/commands.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/options.py` & `doing-cli-1.5.3/src/doing/options.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/pr/commands.py` & `doing-cli-1.5.3/src/doing/pr/commands.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/pr/create_pr.py` & `doing-cli-1.5.3/src/doing/pr/create_pr.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/pr/list_pr.py` & `doing-cli-1.5.3/src/doing/pr/list_pr.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/utils.py` & `doing-cli-1.5.3/src/doing/utils.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing/workon/commands.py` & `doing-cli-1.5.3/src/doing/workon/commands.py`

 * *Files identical despite different names*

### Comparing `doing-cli-1.5.2/src/doing_cli.egg-info/PKG-INFO` & `doing-cli-1.5.3/src/doing_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doing-cli
-Version: 1.5.2
+Version: 1.5.3
 Summary: CLI tool to simplify the development workflow on azure devops
 Home-page: https://github.com/ing-bank/doing-cli
 Author: ING Bank N.V.
 Author-email: tim.vink@ing.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doing-cli-1.5.2/src/doing_cli.egg-info/SOURCES.txt` & `doing-cli-1.5.3/src/doing_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

