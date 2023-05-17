# Comparing `tmp/drtodo-0.5.1.tar.gz` & `tmp/drtodo-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drtodo-0.5.1.tar", max compression
+gzip compressed data, was "drtodo-0.5.2.tar", max compression
```

## Comparing `drtodo-0.5.1.tar` & `drtodo-0.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-04-02 19:49:28.749709 drtodo-0.5.1/LICENSE
--rw-r--r--   0        0        0     9433 2023-05-16 19:07:14.003011 drtodo-0.5.1/drtodo/README.md
--rw-r--r--   0        0        0      224 2023-05-16 17:06:02.545312 drtodo-0.5.1/drtodo/__init__.py
--rw-r--r--   0        0        0       44 2023-05-13 23:41:09.525609 drtodo-0.5.1/drtodo/__main__.py
--rw-r--r--   0        0        0    11865 2023-05-16 18:36:02.348420 drtodo-0.5.1/drtodo/main.py
--rw-r--r--   0        0        0     4679 2023-05-16 18:50:35.678987 drtodo-0.5.1/drtodo/man_command.py
--rw-r--r--   0        0        0     4574 2023-05-16 18:05:33.668663 drtodo-0.5.1/drtodo/mdparser.py
--rw-r--r--   0        0        0     1406 2023-05-16 16:38:13.234806 drtodo-0.5.1/drtodo/mistuneplugin.py
--rw-r--r--   0        0        0      618 2023-05-16 16:11:27.772546 drtodo-0.5.1/drtodo/rich_display.py
--rw-r--r--   0        0        0     7063 2023-05-16 17:04:44.946239 drtodo-0.5.1/drtodo/settings.py
--rw-r--r--   0        0        0       11 2023-04-02 19:49:28.755456 drtodo-0.5.1/drtodo/util.py
--rw-r--r--   0        0        0      657 2023-05-16 18:36:44.693403 drtodo-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    10056 1970-01-01 00:00:00.000000 drtodo-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-02 19:49:28.749709 drtodo-0.5.2/LICENSE
+-rw-r--r--   0        0        0     9429 2023-05-16 21:07:43.881069 drtodo-0.5.2/drtodo/README.md
+-rw-r--r--   0        0        0      224 2023-05-16 17:06:02.545312 drtodo-0.5.2/drtodo/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-13 23:41:09.525609 drtodo-0.5.2/drtodo/__main__.py
+-rw-r--r--   0        0        0    11815 2023-05-17 20:03:17.579930 drtodo-0.5.2/drtodo/main.py
+-rw-r--r--   0        0        0     4681 2023-05-17 21:29:11.605170 drtodo-0.5.2/drtodo/man_command.py
+-rw-r--r--   0        0        0     4718 2023-05-17 21:29:59.622815 drtodo-0.5.2/drtodo/mdparser.py
+-rw-r--r--   0        0        0     1406 2023-05-16 16:38:13.234806 drtodo-0.5.2/drtodo/mistuneplugin.py
+-rw-r--r--   0        0        0      618 2023-05-16 16:11:27.772546 drtodo-0.5.2/drtodo/rich_display.py
+-rw-r--r--   0        0        0     7088 2023-05-17 22:53:38.670275 drtodo-0.5.2/drtodo/settings.py
+-rw-r--r--   0        0        0       11 2023-04-02 19:49:28.755456 drtodo-0.5.2/drtodo/util.py
+-rw-r--r--   0        0        0      709 2023-05-17 21:30:39.963042 drtodo-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    10177 1970-01-01 00:00:00.000000 drtodo-0.5.2/PKG-INFO
```

### Comparing `drtodo-0.5.1/LICENSE` & `drtodo-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drtodo-0.5.1/drtodo/README.md` & `drtodo-0.5.2/drtodo/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# `DrTodo`
+# DrTodo
 
 **DrToDo, MD**: *a straightforward todo list manager for markdown files in git repos.*
 
 ## Quick Start
 
 ### installation
 
@@ -39,15 +39,15 @@
 
 ### use it inside a git repo
 
 > TODO: document this better including the git repo used with `todo init`
 
 ## Contents
 
-- [`DrTodo`](#drtodo)
+- [DrTodo](#drtodo)
   - [Quick Start](#quick-start)
     - [installation](#installation)
     - [initialization](#initialization)
     - [add a todo to the global list](#add-a-todo-to-the-global-list)
     - [list todo items](#list-todo-items)
     - [mark it as done](#mark-it-as-done)
     - [use it inside a git repo](#use-it-inside-a-git-repo)
```

### Comparing `drtodo-0.5.1/drtodo/main.py` & `drtodo-0.5.2/drtodo/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 import re
 from .settings import constants, settings, globals
 from .mdparser import TodoListParser, TaskListTraverser
 from .man_command import manapp
 from .rich_display import console
 
 
-app = typer.Typer(no_args_is_help=True,
-                  rich_markup_mode="markdown",
-                  help="**{constants.appname}, MD**: *a straightforward todo list manager for markdown files in git repos.*",
-                  epilog=f"DrTodo can manage items in a global todo list ({globals.global_todofile_pretty})"
-                  f" and in a local todo list ({globals.local_todofile_pretty or 'if the current folder is under a git repo'})."
-                  f" Settings are read from config files and env variables (see *todo man config*).",
-                  rich_help_panel="Integration")
+app = typer.Typer(
+    no_args_is_help=True,
+    rich_markup_mode="markdown",
+    help="**{constants.appname}, MD**: *a straightforward todo list manager for markdown files in git repos.*",
+    epilog=f"DrTodo can manage items in a global todo list ({globals.global_todofile_pretty})"
+    f" and in a local todo list ({globals.local_todofile_pretty or 'if the current folder is under a git repo'})."
+    f" Settings are read from config files and env variables (see *todo man config*).",
+    rich_help_panel="Integration")
 
 
 def version_string() -> str:
     return f"{constants.appname} v{constants.version}"
 
 
 def ensure_appdir(may_create: bool = False) -> None:
@@ -118,15 +119,16 @@
 @app.command()
 def add(
     description: str,
     priority: int = typer.Option(None, "--priority", "-p"),
     due: str = typer.Option(None, "--due", "-d", help="Due date in any format"),
     owner: str = typer.Option(None, "--owner", "-o", help="Owner userid or name"),
     done: bool = typer.Option(False, "--done", "-D", help="Add item marked as done"),
-    global_todo: bool = typer.Option(False, "--global", "-G", help="Add item to global todo list, even if current folder is under a git repo"),
+    global_todo: bool = typer.Option(False, "--global", "-G",
+                                     help="Add item to global todo list, even if current folder is under a git repo"),
 ):
     """
     Add a new todo item to the list
     """
     duestr = f" due:{due}" if due else ""
     ownerstr = f" @{owner}" if owner else ""
     prioritystr = f" P{priority}" if priority else ""
@@ -140,15 +142,15 @@
         _add_item(todo_item, globals.global_todofile)
     print_todo_item(todo_item)
 
 
 def save_todo_backups(pathname: Path, todo):
     def make_backup_path(i: int) -> Path:
         assert isinstance(i, int) and i > 0
-        # files are hidden and have a '.bak-1' extension for the most recent backup, '.bak-2' for the next most recent, etc.
+        # files are hidden and have a '.bak-1' extension for the most recent backup, '.bak-2' for the next, etc.
         return pathname.with_name(f".{pathname.name.removeprefix('.')}.bak-{i}")
 
     # first write to a temp file with a '.tmp' extension
     tmpfilepath = pathname.with_suffix(pathname.suffix + '.tmp')
     todo.write(tmpfilepath)
 
     # if file write worked, then we can perform the rename dance
@@ -225,30 +227,32 @@
         for item in matching_items_iter(todo.items, id, index, match, all):
             item['checked'] = done
             print_todo_item(item)
         # write back to file
         save_todo_backups(globals.local_todofile, todo)
 
 
-# done [--id <id> | --index <index> | --all | --match <regular expression> | <specification>] (exactly one option must be provided)
+# done [--id <id> | --index <index> | --all | --match <regular expression> | <specification>]
+# (exactly one option must be provided)
 @app.command()
 def done(
     spec: str = typer.Argument(None, help="ID, index or regular expression to match item text"),
     id: str = typer.Option(None, "--id", "-i", help="ID of the item to mark as done"),
     index: int = typer.Option(None, "--index", "-n", help="Index of the item to mark as done"),
     match: str = typer.Option(None, "--match", "-m", help="Regular expression to match item text"),
     all: bool = typer.Option(False, "--all", "-a", help="Mark all items as done"),
 ):
     """
     Mark one or more todo items as done
     """
     _done_undone_marker(True, spec, id, index, match, all)
 
 
-# undone [--id <id> | --index <index> | --all | --match <regular expression> | <specification>] (exactly one option must be provided)
+# undone [--id <id> | --index <index> | --all | --match <regular expression> | <specification>]
+# (exactly one option must be provided)
 @app.command()
 def undone(
     spec: str = typer.Argument(None, help="ID, index or regular expression to match item text"),
     id: str = typer.Option(None, "--id", "-i", help="ID of the item to mark as done"),
     index: int = typer.Option(None, "--index", "-n", help="Index of the item to mark as done"),
     match: str = typer.Option(None, "--match", "-m", help="Regular expression to match item text"),
     all: bool = typer.Option(False, "--all", "-a", help="Mark all items as done"),
```

### Comparing `drtodo-0.5.1/drtodo/man_command.py` & `drtodo-0.5.2/drtodo/man_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 manapp = typer.Typer()
 
 
 def md_mdfiles():
     return f"""
 # Markdown Files
 
-By default, {constants.appname} will look for any lists formatted as GitHub-style task lists in any Markdown files it reads.
+By default, {constants.appname} will look for any lists formatted as GitHub-style task lists in
+any Markdown files it reads.
 
 For example a file containing this:
 ```markdown
 This is my cool project readme file.
 
 ## TODO
 - [x] write a readme
@@ -36,18 +37,19 @@
   1: 5869ea7 ⚫ make it useful
   2: 7a787ec ⚫ bug 1
   3: f237ece ⚫ bug 2
 ```
 
 All items will be logically combined into a single list and listed together.
 
-> In the future, it will be possible to specify which section in a Markdown file to use as a list, and then all other lists
-> will be ignored.
+> In the future, it will be possible to specify which section in a Markdown file to use as a list,
+> and then all other lists will be ignored.
 
-> Also, we will have options to add to the bottom or to the top (meaning right before or right after the last task list item).
+> Also, we will have options to add to the bottom or to the top (meaning right before or right after the
+> last task list item).
 
 """
 
 
 def md_config():
     return f"""
 # Settings
@@ -101,15 +103,16 @@
 hash = 'italic dim yellow'  # color of hash
 text = 'white'              # color of TODO text
 header = 'bold cyan'        # color of header
 warning = 'bold yellow'     # color of warnings
 error = 'red'               # color of errors
 ```
 
-All the colors above use the rich style and color names. See [rich docs](https://rich.readthedocs.io/en/latest/style.html#style) for more info.
+All the colors above use the rich style and color names.
+See [rich docs](https://rich.readthedocs.io/en/latest/style.html#style) for more info.
 
 ## Global Folder
 - `~/.drtodo`                     global config folder
 - `~/.drtodo/config.toml`         global config
 - `~/.drtodo/config.USER.toml`    user specific config (in case this folder is shared)
 - `~/.drtodo/TODO.md`             default location for todo list (configurable, and there could be more)
 - `~/.drtodo/.git`                git repo for todo list (can be shared)
```

### Comparing `drtodo-0.5.1/drtodo/mdparser.py` & `drtodo-0.5.2/drtodo/mdparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import mistune
 from pathlib import Path
 from mistune.renderers.markdown import MarkdownRenderer
-from .mistuneplugin import task_lists, split_task_item
+from .mistuneplugin import task_lists
 
 
 class TokenTraverser:
 
     def traverse_tokens(self, tokens, search_token_type, found_callback):
         for tok in tokens:
             if tok['type'] == search_token_type:
@@ -21,15 +21,18 @@
     @staticmethod
     def calc_git_hash(text):
         import hashlib
         return hashlib.sha1(text.encode('utf-8')).hexdigest()
 
     @staticmethod
     def create_item(text, *, index: int, checked: bool = False, token: dict = None) -> dict:
-        """creates a dict to represent a task list item from text and an index. If token is given, it is used, otherwise a new one is created."""
+        """
+        creates a dict to represent a task list item from text and an index.
+        If token is given, it is used, otherwise a new one is created.
+        """
         id = TaskListTraverser.calc_git_hash(text)
         token = token or TaskListTraverser.create_item_token(checked, text)
         item = {'checked': checked, 'text': text, 'id': id, 'index': index, 'token': token}
         token['task_item'] = item
         return item
 
     @staticmethod
@@ -53,15 +56,18 @@
             if 'task_item' in tok:
                 # already processed in a previous traversal
                 found_items.append(tok['task_item'])
                 return
 
             children = tok['children']
             if children:
-                task_item = self.create_item(tok['attrs']['task_text'], index=len(found_items), checked=tok['attrs']['checked'], token=tok)
+                task_item = self.create_item(tok['attrs']['task_text'],
+                                             index=len(found_items),
+                                             checked=tok['attrs']['checked'],
+                                             token=tok)
                 task_item['parent'] = parent_tokens
                 found_items.append(tok['task_item'])
 
         self.traverse_tokens(tokens, 'list_item', match_task_item)
         return found_items
```

### Comparing `drtodo-0.5.1/drtodo/mistuneplugin.py` & `drtodo-0.5.2/drtodo/mistuneplugin.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.5.1/drtodo/rich_display.py` & `drtodo-0.5.2/drtodo/rich_display.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.5.1/drtodo/settings.py` & `drtodo-0.5.2/drtodo/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
-import os
-from pathlib import Path
+
+import getpass
 from dataclasses import dataclass
-from typing import Any, Optional
+from pathlib import Path
+from typing import Optional, Any, Union
+
 import typer
-from pydantic import BaseSettings, Field, BaseModel
+from pydantic import BaseModel, BaseSettings, Field
+
 try:
     import tomllib as toml
 except ImportError:
     import tomli as toml
 from git import Repo
-from . import __version__
 
+from . import __version__
 
 __all__ = ["constants", "settings", "globals", "initialize", "make_pretty_path"]
 
 
 @dataclass(frozen=True)
 class Constants:
     appname: str = "DrTodo"
     appdir: Path = Path(typer.get_app_dir(appname, force_posix=True))
     version: str = __version__
     env_prefix = appname.upper() + "_"
-    username: str = os.getlogin()
+    username: str = getpass.getuser()
 
 
 constants: Constants = Constants()
 
 
 class Style(BaseModel):
     checked: str = '🔘'
@@ -54,15 +57,15 @@
 
 
 class Settings(BaseSettings):
     mdfile: str = Field("TODO.md", env=constants.env_prefix + "MDFILE")
     verbose: bool = False
     keep_backups: int = 3   # number of backups to keep
     hide_hash: bool = False
-    style: Style | str = ''
+    style: Union[Style, str] = ''
 
     # def __init__(self, **kwargs):
     #     super().__init__(**kwargs)
     #     self.update_values()
 
     def update_values(self):
         if isinstance(self.style, str):
```

### Comparing `drtodo-0.5.1/PKG-INFO` & `drtodo-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: drtodo
-Version: 0.5.1
+Version: 0.5.2
 Summary: DrTodo, MD: todo list manager using markdown files and git
 License: MIT
 Author: exilium
 Author-email: info@exilium.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gitpython
 Requires-Dist: mistune (==3.0.0rc5)
 Requires-Dist: pydantic
-Requires-Dist: pygithub
 Requires-Dist: rich
-Requires-Dist: ruamel.yaml
 Requires-Dist: tomli ; python_version < "3.11"
 Requires-Dist: typer
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.11"
 Description-Content-Type: text/markdown
 
-# `DrTodo`
+# DrTodo
 
 **DrToDo, MD**: *a straightforward todo list manager for markdown files in git repos.*
 
 ## Quick Start
 
 ### installation
 
@@ -60,15 +61,15 @@
 
 ### use it inside a git repo
 
 > TODO: document this better including the git repo used with `todo init`
 
 ## Contents
 
-- [`DrTodo`](#drtodo)
+- [DrTodo](#drtodo)
   - [Quick Start](#quick-start)
     - [installation](#installation)
     - [initialization](#initialization)
     - [add a todo to the global list](#add-a-todo-to-the-global-list)
     - [list todo items](#list-todo-items)
     - [mark it as done](#mark-it-as-done)
     - [use it inside a git repo](#use-it-inside-a-git-repo)
```

