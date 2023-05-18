# Comparing `tmp/browsr-1.7.0.tar.gz` & `tmp/browsr-1.8.0.tar.gz`

## Comparing `browsr-1.7.0.tar` & `browsr-1.8.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 browsr-1.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.7.0/.releaserc.js
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 browsr-1.7.0/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/__main__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_base.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_cli.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_config.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_tools.py
--rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_version.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/browsr.css
--rw-r--r--   0        0        0    13149 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/browsr.py
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/universal_directory_tree.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/contributing.md
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/index.md
--rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/browsr.png
--rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/browsr_no_label.png
--rw-r--r--   0        0        0  2345036 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/screenshot_datatable.png
--rw-r--r--   0        0        0  1798671 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/screenshot_markdown.png
--rw-r--r--   0        0        0  2487884 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/screenshot_mona_lisa.png
--rw-r--r--   0        0        0  2059371 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/screenshot_utils.png
--rw-r--r--   0        0        0   124812 2020-02-02 00:00:00.000000 browsr-1.7.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    82506 2020-02-02 00:00:00.000000 browsr-1.7.0/requirements/requirements-prod.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/conftest.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/helpers.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/test_cli.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/test_screenshots.py
--rw-r--r--   0        0        0     8069 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/cassettes/test_github_screenshot.yaml
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/cassettes/test_github_screenshot_license.yaml
--rw-r--r--   0        0        0    62231 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/screenshots/test_github_screenshot.svg
--rw-r--r--   0        0        0    47130 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/screenshots/test_github_screenshot_license.svg
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.7.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.7.0/LICENSE
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 browsr-1.7.0/README.md
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 browsr-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 browsr-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 browsr-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.8.0/.releaserc.js
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 browsr-1.8.0/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.8.0/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/__main__.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_base.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_cli.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_config.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_tools.py
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/_version.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/browsr.css
+-rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/browsr.py
+-rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 browsr-1.8.0/browsr/universal_directory_tree.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/contributing.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/index.md
+-rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/browsr.png
+-rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/browsr_no_label.png
+-rw-r--r--   0        0        0  2345036 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/screenshot_datatable.png
+-rw-r--r--   0        0        0  1798671 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/screenshot_markdown.png
+-rw-r--r--   0        0        0  2487884 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/screenshot_mona_lisa.png
+-rw-r--r--   0        0        0  2059371 2020-02-02 00:00:00.000000 browsr-1.8.0/docs/_static/screenshot_utils.png
+-rw-r--r--   0        0        0   124812 2020-02-02 00:00:00.000000 browsr-1.8.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    82506 2020-02-02 00:00:00.000000 browsr-1.8.0/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/helpers.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/test_config.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/test_screenshots.py
+-rw-r--r--   0        0        0    12523 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/cassettes/test_github_screenshot.yaml
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/cassettes/test_github_screenshot_license.yaml
+-rw-r--r--   0        0        0    35329 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/cassettes/test_textual_app_context_path_github.yaml
+-rw-r--r--   0        0        0    62231 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/screenshots/test_github_screenshot.svg
+-rw-r--r--   0        0        0    47130 2020-02-02 00:00:00.000000 browsr-1.8.0/tests/screenshots/test_github_screenshot_license.svg
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.8.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.8.0/LICENSE
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 browsr-1.8.0/README.md
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 browsr-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 browsr-1.8.0/PKG-INFO
```

### Comparing `browsr-1.7.0/.pre-commit-config.yaml` & `browsr-1.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/.releaserc.js` & `browsr-1.8.0/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/mkdocs.yaml` & `browsr-1.8.0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/.github/semantic_release/package-lock.json` & `browsr-1.8.0/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/.github/semantic_release/release_notes.hbs` & `browsr-1.8.0/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/.github/workflows/lint.yaml` & `browsr-1.8.0/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/.github/workflows/publish.yaml` & `browsr-1.8.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/.github/workflows/release.yaml` & `browsr-1.8.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/.github/workflows/tests.yaml` & `browsr-1.8.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/browsr/_base.py` & `browsr-1.8.0/browsr/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,18 +39,24 @@
     max_file_size: int = 20
 
     @property
     def path(self) -> pathlib.Path:
         """
         Resolve `file_path` to a upath.UPath object
         """
+        if "github" in str(self.file_path).lower():
+            file_path = str(self.file_path)
+            file_path = file_path.lstrip("https://")
+            file_path = file_path.lstrip("http://")
+            file_path = file_path.lstrip("www.")
+            file_path = file_path.rstrip(".git")
+            file_path = handle_github_url(url=str(file_path))
+            self.file_path = file_path
         if str(self.file_path).endswith("/"):
             self.file_path = str(self.file_path)[:-1]
-        if "github" in str(self.file_path):
-            self.file_path = handle_github_url(url=str(self.file_path))
         return (
             upath.UPath(self.file_path).resolve()
             if self.file_path
             else pathlib.Path.cwd().resolve()
         )
```

### Comparing `browsr-1.7.0/browsr/_cli.py` & `browsr-1.8.0/browsr/_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -68,38 +68,81 @@
 
     ```shell
     pipx install "browsr[all]"
     ```
 
     ## Usage Examples
 
-    - Load your current working directory
-        ```shell
-        browsr
-        ```
-    - Load a local directory
-        ```shell
-        browsr/path/to/directory
-        ```
-    - Load an S3 bucket
-        ```shell
-        browsr s3://bucket-name
-        ```
-    - Load a GCS bucket
-        ```shell
-        browsr gs://bucket-name
-        ```
-    - Load a GitHub repository
-        ```shell
-        browsr github://juftin:browsr
-        ```
-    - Load a GitHub repository branch
-        ```shell
-        browsr github://juftin:browsr@main
-        ```
+    ### Local
+
+    #### Browse your current working directory
+
+    ```shell
+    browsr
+    ```
+
+    #### Browse a local directory
+
+    ```shell
+    browsr/path/to/directory
+    ```
+
+    ### Cloud Storage
+
+    #### Browse an S3 bucket
+
+    ```shell
+    browsr s3://bucket-name
+    ```
+
+    #### Browse a GCS bucket
+
+    ```shell
+    browsr gs://bucket-name
+    ```
+
+    #### Browse Azure Services
+
+    ```shell
+    browsr adl://bucket-name
+    browsr az://bucket-name
+    ```
+
+    ### GitHub
+
+    #### Browse a GitHub repository
+
+    ```shell
+    browsr github://juftin:browsr
+    ```
+
+    #### Browse a GitHub Repository Branch
+
+    ```shell
+    browsr github://juftin:browsr@main
+    ```
+
+    #### Browse a Private GitHub Repository
+
+    ```shell
+    export GITHUB_TOKEN="ghp_1234567890"
+    browsr github://juftin:browsr-private@main
+    ```
+
+    #### Browse a GitHub Repository Subdirectory
+
+    ```shell
+    browsr github://juftin:browsr@main/tests
+    ```
+
+    #### Browse a GitHub URL
+
+    ```shell
+    browsr https://github.com/juftin/browsr
+    ```
 
     ## Key Bindings
     - **`Q`** - Quit the application
     - **`F`** - Toggle the file tree sidebar
     - **`T`** - Toggle the rich theme for code formatting
     - **`N`** - Toggle line numbers for code formatting
     - **`D`** - Toggle dark mode for the application
```

### Comparing `browsr-1.7.0/browsr/_config.py` & `browsr-1.8.0/browsr/_config.py`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/browsr/_tools.py` & `browsr-1.8.0/browsr/_tools.py`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/browsr/_utils.py` & `browsr-1.8.0/browsr/_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -136,18 +136,22 @@
     GitHub URLs are handled by converting them to the raw URL.
     """
     if "github://" in url and "@" not in url:
         _, user_password = url.split("github://")
         org, repo = user_password.split(":")
     elif "github://" in url and "@" in url:
         return url
-    elif "github.com" in url and "https" in url:
-        _, url = url.split("://")
+    elif "github.com" in url.lower():
         _, org, repo, *args = url.split("/")
+    else:
+        raise ValueError(f"Invalid GitHub URL: {url}")
+    token = os.getenv("GITHUB_TOKEN")
+    auth = {"auth": ("Bearer", token)} if token is not None else {}
     resp = requests.get(
         f"https://api.github.com/repos/{org}/{repo}",
         headers={"Accept": "application/vnd.github.v3+json"},
+        **auth,  # type: ignore[arg-type]
     )
     resp.raise_for_status()
     default_branch = resp.json()["default_branch"]
     github_uri = f"github://{org}:{repo}@{default_branch}"
     return github_uri
```

### Comparing `browsr-1.7.0/browsr/browsr.css` & `browsr-1.8.0/browsr/browsr.css`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/browsr/browsr.py` & `browsr-1.8.0/browsr/browsr.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 This module contains the code browser app for the browsr package.
 This app was inspired by the CodeBrowser example from textual
 """
 
 import json
 import pathlib
 import shutil
+from os import getenv
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Iterable, Optional, Union
 
 import pandas as pd
 import upath
 from art import text2art  # type: ignore[import]
 from rich.markdown import Markdown
@@ -352,11 +353,13 @@
             self.confirmation.download_message.update(Markdown(prompt_message))
             self.confirmation.refresh()
             self.hidden_table_view = self.table_view.display
             self.table_view.display = False
             self.confirmation_window.display = True
 
 
-app = Browsr(config_object=TextualAppContext(file_path=None, debug=True))
+app = Browsr(
+    config_object=TextualAppContext(file_path=getenv("BROWSR_PATH"), debug=True)
+)
 
 if __name__ == "__main__":
     app.run()
```

### Comparing `browsr-1.7.0/browsr/universal_directory_tree.py` & `browsr-1.8.0/browsr/universal_directory_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 A universal directory tree widget for Textual.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
+from os import getenv
 from typing import Any, ClassVar, Iterable, Optional
 
 import upath
 from textual.events import Mount
 from textual.reactive import var
 from textual.widgets import DirectoryTree
 from textual.widgets._tree import Tree, TreeNode
@@ -154,14 +155,23 @@
     """
     GitHubPath
 
     UPath implementation for GitHub to be compatible with
     the Universal Directory Tree
     """
 
+    def __new__(cls, *args, **kwargs) -> "GitHubPath":  # type: ignore[no-untyped-def]
+        """
+        Attempt to set the username and token from the environment
+        """
+        token = getenv("GITHUB_TOKEN")
+        kwargs.update({"username": "Bearer", "token": token})
+        github_path = super().__new__(cls, *args, **kwargs)
+        return github_path
+
     @property
     def path(self) -> str:
         """
         Paths get their leading slash stripped
         """
         return super().path.strip("/")
```

### Comparing `browsr-1.7.0/docs/contributing.md` & `browsr-1.8.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/docs/gen_ref_pages.py` & `browsr-1.8.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/docs/index.md` & `browsr-1.8.0/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,19 @@
 
 ### GitHub
 
 ```
 browsr github://juftin:browsr
 ```
 
+```
+export GITHUB_TOKEN="ghp_1234567890"
+browsr github://juftin:browsr-private@main
+```
+
 ### Cloud
 
 ```shell
 browsr s3://my-bucket
 ```
 
 ** _Currently AWS S3, Google Cloud Storage, and Azure Blob Storage are supported._
```

#### html2text {}

```diff
@@ -29,9 +29,11 @@
 systems, like GitHub or AWS S3, you'll need to install the `remote` extra. If
 you'd like to browse parquet files, you'll need to install the `parquet` extra.
 Or, even simpler, you can install the `all` extra to get all the extras.
 ```shell pipx install "browsr[all]" ``` ## Usage Simply give **`browsr`** a
 path to a local or remote file / directory. [Check out the Documentation]
 (https://juftin.com/browsr/) for more information about the file systems
 supported. ### Local ```shell browsr ~/Downloads/ ``` ### GitHub ``` browsr
-github://juftin:browsr ``` ### Cloud ```shell browsr s3://my-bucket ``` **
-_Currently AWS S3, Google Cloud Storage, and Azure Blob Storage are supported._
+github://juftin:browsr ``` ``` export GITHUB_TOKEN="ghp_1234567890" browsr
+github://juftin:browsr-private@main ``` ### Cloud ```shell browsr s3://my-
+bucket ``` ** _Currently AWS S3, Google Cloud Storage, and Azure Blob Storage
+are supported._
```

### Comparing `browsr-1.7.0/docs/_static/browsr.png` & `browsr-1.8.0/docs/_static/browsr.png`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/docs/_static/browsr_no_label.png` & `browsr-1.8.0/docs/_static/browsr_no_label.png`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/docs/_static/screenshot_datatable.png` & `browsr-1.8.0/docs/_static/screenshot_datatable.png`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/docs/_static/screenshot_markdown.png` & `browsr-1.8.0/docs/_static/screenshot_markdown.png`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/docs/_static/screenshot_mona_lisa.png` & `browsr-1.8.0/docs/_static/screenshot_mona_lisa.png`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/docs/_static/screenshot_utils.png` & `browsr-1.8.0/docs/_static/screenshot_utils.png`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/requirements/requirements-dev.txt` & `browsr-1.8.0/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/requirements/requirements-prod.txt` & `browsr-1.8.0/requirements/requirements-prod.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/tests/conftest.py` & `browsr-1.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/tests/helpers.py` & `browsr-1.8.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/tests/test_screenshots.py` & `browsr-1.8.0/tests/test_screenshots.py`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/tests/cassettes/test_github_screenshot.yaml` & `browsr-1.8.0/tests/cassettes/test_github_screenshot.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -45,19 +45,19 @@
               Content-Length:
                   - "728"
               Content-Security-Policy:
                   - default-src 'none'
               Content-Type:
                   - application/json; charset=utf-8
               Date:
-                  - Wed, 17 May 2023 21:30:44 GMT
+                  - Thu, 18 May 2023 01:01:44 GMT
               ETag:
                   - W/"91ee3d202828b3c28fcd9be69924424a4f792f5f17ff608d6d4ac2b1e19e5fcd"
               Last-Modified:
-                  - Wed, 17 May 2023 21:16:30 GMT
+                  - Wed, 17 May 2023 23:39:58 GMT
               Referrer-Policy:
                   - origin-when-cross-origin, strict-origin-when-cross-origin
               Server:
                   - GitHub.com
               Strict-Transport-Security:
                   - max-age=31536000; includeSubdomains; preload
               Vary:
@@ -65,25 +65,120 @@
               X-Content-Type-Options:
                   - nosniff
               X-Frame-Options:
                   - deny
               X-GitHub-Media-Type:
                   - github.v3; format=json
               X-GitHub-Request-Id:
-                  - CEAA:5DE3:FF9051:20DD28A:64654784
+                  - C66F:5F92:13EA1B3:28FFF1A:646578F8
               X-RateLimit-Limit:
                   - "60"
               X-RateLimit-Remaining:
-                  - "42"
+                  - "53"
               X-RateLimit-Reset:
-                  - "1684359062"
+                  - "1684374609"
               X-RateLimit-Resource:
                   - core
               X-RateLimit-Used:
-                  - "18"
+                  - "7"
+              X-XSS-Protection:
+                  - "0"
+              x-github-api-version-selected:
+                  - "2022-11-28"
+          status:
+              code: 200
+              message: OK
+    - request:
+          body: null
+          headers:
+              Accept:
+                  - "*/*"
+              Accept-Encoding:
+                  - gzip, deflate
+              Connection:
+                  - keep-alive
+              User-Agent:
+                  - python-requests/2.28.2
+              authorization:
+                  - XXXXXXXXXX
+          method: GET
+          uri: https://api.github.com/repos/juftin/browsr/git/trees/v1.6.0
+      response:
+          body:
+              string: !!binary |
+                  H4sIAAAAAAAAA6WWTW/bOBCG/4vOqcXh5zC3YjeHBdoetsdiDzPkMHHWtlxJxiIt8t9LbYJavRRs
+                  5YNtQiYeP+TwHX7tpgfqbjtGJQTRBBe0siBaMqItJkOIECkYbVmh4u6mu4yHOuFhns/Tbd/Teb+7
+                  388PF96l4diPch6m/vFS5v2p53H4bxr7+rifR5Gp/wXKMqG7/fS1O9P8UHmvkMo/Drk+6ZRV9VXH
+                  89N5Gf8/4eZVh6ICkhw92yBJSpbiuRhnFDqvvKPgS4kFt+k0U55vfvDY35+GcfmzryqglLf2qsKH
+                  YVnol50JorLN1ikyjmIwkl0dgwgHG9FDKexRUlkm7L/UldCo7G/u0gKe+mbiWus8yptaAMf9XD9O
+                  ZX+/e6LjodGRYsagLGFCByCerFHKaEnag0smlypbGJclenEEE+Imx2bi2nGUg9AkY9o9To1mAYQ5
+                  m2riIDjkEsVQ8gxJW48KqcSsMdLVzIWNu9dKXJm9++uPuw8f7xqdTAEAnzmmRExogApnG5zVhJml
+                  QBLWgPHqBGrbbjUTV05/37398/3d7pgbrYCD1kEjCFCKiqPySTlCnSR6ZJ+dGACbrues/nhTDTYT
+                  V1YvkXpV+mkK5myLYvJoEDnVdw1asTdIYG0MTCWbaN3GUG+mrDTykFYn6OcSddlzzQWyYAoWnXKu
+                  LckoXSOcKDmJRkpKS7Vt6Ey5lbKSOP67aPxKzmUHrgZ2AetAAaRMNRdsMsE6ASehxkEItRdcawzQ
+                  /KbXS5Y3E1de56fzODxKmnfz0BzhEVm8AsQl5GxKBTIVCk7FXKtPqDZeEySH72rW2m3Hp5m4Uhvl
+                  82U/ylFOc2v9GVbW5kIpJ1Y159jkyLU5GV8vR8Ylh9GKheUmsqH+mikrmVmmZotaZw6xGIGYtBLx
+                  aGtGOweZgzeO61c2qWw8Rc2U53/qvW28nBLNkrvbQodJnr8BMK8OzowKAAA=
+          headers:
+              Access-Control-Allow-Origin:
+                  - "*"
+              Access-Control-Expose-Headers:
+                  - ETag, Link, Location, Retry-After, X-GitHub-OTP, X-RateLimit-Limit, X-RateLimit-Remaining,
+                    X-RateLimit-Used, X-RateLimit-Resource, X-RateLimit-Reset, X-OAuth-Scopes,
+                    X-Accepted-OAuth-Scopes, X-Poll-Interval, X-GitHub-Media-Type, X-GitHub-SSO,
+                    X-GitHub-Request-Id, Deprecation, Sunset
+              Cache-Control:
+                  - private, max-age=60, s-maxage=60
+              Content-Encoding:
+                  - gzip
+              Content-Security-Policy:
+                  - default-src 'none'
+              Content-Type:
+                  - application/json; charset=utf-8
+              Date:
+                  - Thu, 18 May 2023 01:01:44 GMT
+              ETag:
+                  - W/"020b9c645dc6800fbd32a722b2d8f51d3a58cc017d63e5da3554a56489b157ec"
+              Last-Modified:
+                  - Wed, 17 May 2023 23:39:58 GMT
+              Referrer-Policy:
+                  - origin-when-cross-origin, strict-origin-when-cross-origin
+              Server:
+                  - GitHub.com
+              Strict-Transport-Security:
+                  - max-age=31536000; includeSubdomains; preload
+              Transfer-Encoding:
+                  - chunked
+              Vary:
+                  - Accept, Authorization, Cookie, X-GitHub-OTP
+                  - Accept-Encoding, Accept, X-Requested-With
+              X-Accepted-OAuth-Scopes:
+                  - ""
+              X-Content-Type-Options:
+                  - nosniff
+              X-Frame-Options:
+                  - deny
+              X-GitHub-Media-Type:
+                  - github.v3; format=json
+              X-GitHub-Request-Id:
+                  - C670:14FC:14A1CE8:2A6CA7E:646578F8
+              X-OAuth-Scopes:
+                  - admin:gpg_key, admin:org, admin:org_hook, admin:public_key, admin:repo_hook,
+                    admin:ssh_signing_key, audit_log, codespace, delete:packages, gist, notifications,
+                    project, read:enterprise, repo, user, workflow, write:discussion, write:packages
+              X-RateLimit-Limit:
+                  - "5000"
+              X-RateLimit-Remaining:
+                  - "4981"
+              X-RateLimit-Reset:
+                  - "1684373394"
+              X-RateLimit-Resource:
+                  - core
+              X-RateLimit-Used:
+                  - "19"
               X-XSS-Protection:
                   - "0"
               x-github-api-version-selected:
                   - "2022-11-28"
           status:
               code: 200
               message: OK
@@ -137,42 +232,42 @@
               Content-Length:
                   - "1101"
               Content-Security-Policy:
                   - default-src 'none'; style-src 'unsafe-inline'; sandbox
               Content-Type:
                   - text/plain; charset=utf-8
               Date:
-                  - Wed, 17 May 2023 21:30:44 GMT
+                  - Thu, 18 May 2023 01:01:44 GMT
               ETag:
                   - W/"e3f73ab855fd90588244244759492697dae0221aaa9e819693338d2cd1ad119e"
               Expires:
-                  - Wed, 17 May 2023 21:35:44 GMT
+                  - Thu, 18 May 2023 01:06:44 GMT
               Source-Age:
                   - "0"
               Strict-Transport-Security:
                   - max-age=31536000
               Vary:
                   - Authorization,Accept-Encoding,Origin
               Via:
                   - 1.1 varnish
               X-Cache:
-                  - HIT
+                  - MISS
               X-Cache-Hits:
-                  - "1"
+                  - "0"
               X-Content-Type-Options:
                   - nosniff
               X-Fastly-Request-ID:
-                  - 8db268a9faffcad81d0b18decbadb968a115ce12
+                  - 7459b3f705b11601e933e9db121561cfa0dae324
               X-Frame-Options:
                   - deny
               X-GitHub-Request-Id:
-                  - 5E1C:093A:1CF866C:221F6FC:646545DF
+                  - F40E:6E4E:3A21014:443B1B9:646578F8
               X-Served-By:
-                  - cache-den8228-DEN
+                  - cache-den8272-DEN
               X-Timer:
-                  - S1684359045.859318,VS0,VE120
+                  - S1684371705.820747,VS0,VE131
               X-XSS-Protection:
                   - 1; mode=block
           status:
               code: 200
               message: OK
 version: 1
```

### Comparing `browsr-1.7.0/tests/cassettes/test_github_screenshot_license.yaml` & `browsr-1.8.0/tests/cassettes/test_github_screenshot_license.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -41,42 +41,42 @@
               Content-Length:
                   - "664"
               Content-Security-Policy:
                   - default-src 'none'; style-src 'unsafe-inline'; sandbox
               Content-Type:
                   - text/plain; charset=utf-8
               Date:
-                  - Wed, 17 May 2023 22:18:05 GMT
+                  - Thu, 18 May 2023 01:01:45 GMT
               ETag:
                   - W/"7317880eca0696f93222e0968307748f383c87a2a37112679931db91bdd5f000"
               Expires:
-                  - Wed, 17 May 2023 22:23:05 GMT
+                  - Thu, 18 May 2023 01:06:45 GMT
               Source-Age:
                   - "0"
               Strict-Transport-Security:
                   - max-age=31536000
               Vary:
                   - Authorization,Accept-Encoding,Origin
               Via:
                   - 1.1 varnish
               X-Cache:
-                  - HIT
+                  - MISS
               X-Cache-Hits:
-                  - "1"
+                  - "0"
               X-Content-Type-Options:
                   - nosniff
               X-Fastly-Request-ID:
-                  - 42e5a40071fd4ee6de7a60bc4d1ee42e41a1b3a5
+                  - d2531263c424560513b093dc95b27b5d1046121c
               X-Frame-Options:
                   - deny
               X-GitHub-Request-Id:
-                  - E4AE:7A76:1C7A999:21A49D2:64654B2B
+                  - B520:0A4A:1931F94:1D9B25C:646578F9
               X-Served-By:
-                  - cache-den8280-DEN
+                  - cache-den8283-DEN
               X-Timer:
-                  - S1684361886.730164,VS0,VE120
+                  - S1684371705.312640,VS0,VE131
               X-XSS-Protection:
                   - 1; mode=block
           status:
               code: 200
               message: OK
 version: 1
```

### Comparing `browsr-1.7.0/tests/screenshots/test_github_screenshot.svg` & `browsr-1.8.0/tests/screenshots/test_github_screenshot.svg`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/tests/screenshots/test_github_screenshot_license.svg` & `browsr-1.8.0/tests/screenshots/test_github_screenshot_license.svg`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/.gitignore` & `browsr-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/LICENSE` & `browsr-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browsr-1.7.0/README.md` & `browsr-1.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,19 @@
 
 ### GitHub
 
 ```
 browsr github://juftin:browsr
 ```
 
+```
+export GITHUB_TOKEN="ghp_1234567890"
+browsr github://juftin:browsr-private@main
+```
+
 ### Cloud
 
 ```shell
 browsr s3://my-bucket
 ```
 
 \*\* _Currently AWS S3, Google Cloud Storage, and Azure Blob Storage are supported._
```

#### html2text {}

```diff
@@ -27,11 +27,12 @@
 If you're looking to use **`browsr`** on remote file systems, like GitHub or
 AWS S3, you'll need to install the `remote` extra. If you'd like to browse
 parquet files, you'll need to install the `parquet` extra. Or, even simpler,
 you can install the `all` extra to get all the extras. ```shell pipx install
 "browsr[all]" ``` ## Usage Simply give **`browsr`** a path to a local or remote
 file / directory. [Check out the Documentation](https://juftin.com/browsr/) for
 more information about the file systems supported. ### Local ```shell browsr ~/
-Downloads/ ``` ### GitHub ``` browsr github://juftin:browsr ``` ### Cloud
-```shell browsr s3://my-bucket ``` \*\* _Currently AWS S3, Google Cloud
-Storage, and Azure Blob Storage are supported._ ## License **`browsr`** is
-distributed under the terms of the [MIT license](LICENSE).
+Downloads/ ``` ### GitHub ``` browsr github://juftin:browsr ``` ``` export
+GITHUB_TOKEN="ghp_1234567890" browsr github://juftin:browsr-private@main ```
+### Cloud ```shell browsr s3://my-bucket ``` \*\* _Currently AWS S3, Google
+Cloud Storage, and Azure Blob Storage are supported._ ## License **`browsr`**
+is distributed under the terms of the [MIT license](LICENSE).
```

### Comparing `browsr-1.7.0/pyproject.toml` & `browsr-1.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,17 @@
   "pip-tools~=6.13.0",
   "textual[dev]~=0.24.1"
 ]
 features = ["all"]
 pre-install-commands = ["pip install -U --no-deps -r requirements/requirements-dev.txt"]
 python = "3.10"
 
+[tool.hatch.envs.default.env-vars]
+GITHUB_TOKEN = "{env:GITHUB_TOKEN:placeholder}"
+
 [tool.hatch.envs.default.scripts]
 _pip_compile = "pip-compile --resolver=backtracking --generate-hashes requirements.in"
 all = ["format", "lint", "check", "test"]
 check = [
   "mypy --install-types --strict-optional --non-interactive {args:browsr/ tests/}"
 ]
 docs-build = ["mkdocs build --clean --strict"]
@@ -147,15 +150,16 @@
 ignore_errors = true
 module = [
   "rich_click.*"
 ]
 
 [tool.ruff]
 ignore = [
-  "E501"  # line too long, handled by black
+  "E501",  # line too long, handled by black
+  "B005"  # Using `.strip()` with multi-character strings is misleading the reader
 ]
 select = [
   "E",  # pycodestyle errors
   "W",  # pycodestyle warnings
   "F",  # pyflakes
   "I",  # isort
   "C",  # flake8-comprehensions
```

### Comparing `browsr-1.7.0/PKG-INFO` & `browsr-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browsr
-Version: 1.7.0
+Version: 1.8.0
 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme
 Project-URL: Issues, https://github.com/juftin/browsr/issues
 Project-URL: Source, https://github.com/juftin/browsr
 Author-email: Justin Flannery <justin.flannery@juftin.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -122,14 +122,19 @@
 
 ### GitHub
 
 ```
 browsr github://juftin:browsr
 ```
 
+```
+export GITHUB_TOKEN="ghp_1234567890"
+browsr github://juftin:browsr-private@main
+```
+
 ### Cloud
 
 ```shell
 browsr s3://my-bucket
 ```
 
 \*\* _Currently AWS S3, Google Cloud Storage, and Azure Blob Storage are supported._
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: browsr Version: 1.7.0 Summary: TUI File Browser App
+Metadata-Version: 2.1 Name: browsr Version: 1.8.0 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme Project-
 URL: Issues, https://github.com/juftin/browsr/issues Project-URL: Source,
 https://github.com/juftin/browsr Author-email: Justin Flannery
 flannery@juftin.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -49,11 +49,12 @@
 If you're looking to use **`browsr`** on remote file systems, like GitHub or
 AWS S3, you'll need to install the `remote` extra. If you'd like to browse
 parquet files, you'll need to install the `parquet` extra. Or, even simpler,
 you can install the `all` extra to get all the extras. ```shell pipx install
 "browsr[all]" ``` ## Usage Simply give **`browsr`** a path to a local or remote
 file / directory. [Check out the Documentation](https://juftin.com/browsr/) for
 more information about the file systems supported. ### Local ```shell browsr ~/
-Downloads/ ``` ### GitHub ``` browsr github://juftin:browsr ``` ### Cloud
-```shell browsr s3://my-bucket ``` \*\* _Currently AWS S3, Google Cloud
-Storage, and Azure Blob Storage are supported._ ## License **`browsr`** is
-distributed under the terms of the [MIT license](LICENSE).
+Downloads/ ``` ### GitHub ``` browsr github://juftin:browsr ``` ``` export
+GITHUB_TOKEN="ghp_1234567890" browsr github://juftin:browsr-private@main ```
+### Cloud ```shell browsr s3://my-bucket ``` \*\* _Currently AWS S3, Google
+Cloud Storage, and Azure Blob Storage are supported._ ## License **`browsr`**
+is distributed under the terms of the [MIT license](LICENSE).
```

