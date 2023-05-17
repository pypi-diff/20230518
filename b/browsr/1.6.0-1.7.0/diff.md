# Comparing `tmp/browsr-1.6.0.tar.gz` & `tmp/browsr-1.7.0.tar.gz`

## Comparing `browsr-1.6.0.tar` & `browsr-1.7.0.tar`

### file list

```diff
@@ -1,43 +1,50 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.6.0/.releaserc.js
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 browsr-1.6.0/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/__main__.py
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_base.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_cli.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_config.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_tools.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_version.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/browsr.css
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/browsr.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/universal_directory_tree.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/contributing.md
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/index.md
--rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/browsr.png
--rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/browsr_no_label.png
--rw-r--r--   0        0        0  2345036 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/screenshot_datatable.png
--rw-r--r--   0        0        0  1798671 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/screenshot_markdown.png
--rw-r--r--   0        0        0  2487884 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/screenshot_mona_lisa.png
--rw-r--r--   0        0        0  2059371 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/screenshot_utils.png
--rw-r--r--   0        0        0   124300 2020-02-02 00:00:00.000000 browsr-1.6.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    82506 2020-02-02 00:00:00.000000 browsr-1.6.0/requirements/requirements-prod.txt
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 browsr-1.6.0/tests/conftest.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.6.0/tests/test_cli.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.6.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.6.0/LICENSE
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 browsr-1.6.0/README.md
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 browsr-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 browsr-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 browsr-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.7.0/.releaserc.js
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 browsr-1.7.0/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.7.0/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/__main__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_base.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_cli.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_config.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_tools.py
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/_version.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/browsr.css
+-rw-r--r--   0        0        0    13149 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/browsr.py
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 browsr-1.7.0/browsr/universal_directory_tree.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/contributing.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/index.md
+-rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/browsr.png
+-rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/browsr_no_label.png
+-rw-r--r--   0        0        0  2345036 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/screenshot_datatable.png
+-rw-r--r--   0        0        0  1798671 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/screenshot_markdown.png
+-rw-r--r--   0        0        0  2487884 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/screenshot_mona_lisa.png
+-rw-r--r--   0        0        0  2059371 2020-02-02 00:00:00.000000 browsr-1.7.0/docs/_static/screenshot_utils.png
+-rw-r--r--   0        0        0   124812 2020-02-02 00:00:00.000000 browsr-1.7.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    82506 2020-02-02 00:00:00.000000 browsr-1.7.0/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/helpers.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/test_cli.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/test_screenshots.py
+-rw-r--r--   0        0        0     8069 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/cassettes/test_github_screenshot.yaml
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/cassettes/test_github_screenshot_license.yaml
+-rw-r--r--   0        0        0    62231 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/screenshots/test_github_screenshot.svg
+-rw-r--r--   0        0        0    47130 2020-02-02 00:00:00.000000 browsr-1.7.0/tests/screenshots/test_github_screenshot_license.svg
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.7.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.7.0/LICENSE
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 browsr-1.7.0/README.md
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 browsr-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 browsr-1.7.0/PKG-INFO
```

### Comparing `browsr-1.6.0/.pre-commit-config.yaml` & `browsr-1.7.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 fail_fast: false
 
 repos:
     - repo: https://github.com/pre-commit/pre-commit-hooks
       rev: v4.4.0
       hooks:
           - id: trailing-whitespace
+            exclude: '\.svg$'
           - id: end-of-file-fixer
           - id: check-yaml
           - id: check-ast
           - id: check-docstring-first
           - id: check-merge-conflict
           - id: mixed-line-ending
```

### Comparing `browsr-1.6.0/.releaserc.js` & `browsr-1.7.0/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/mkdocs.yaml` & `browsr-1.7.0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/.github/semantic_release/package-lock.json` & `browsr-1.7.0/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/.github/semantic_release/release_notes.hbs` & `browsr-1.7.0/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/.github/workflows/lint.yaml` & `browsr-1.7.0/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/.github/workflows/publish.yaml` & `browsr-1.7.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/.github/workflows/release.yaml` & `browsr-1.7.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/.github/workflows/tests.yaml` & `browsr-1.7.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/browsr/_base.py` & `browsr-1.7.0/browsr/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from textual.app import App, ComposeResult
 from textual.containers import Container
 from textual.reactive import reactive, var
 from textual.widget import Widget
 from textual.widgets import Button, DataTable, Static
 
 from browsr._config import favorite_themes
-from browsr._utils import FileInfo
+from browsr._utils import FileInfo, handle_github_url
 
 
 @dataclass
 class TextualAppContext:
     """
     App Context Object
     """
@@ -41,14 +41,16 @@
     @property
     def path(self) -> pathlib.Path:
         """
         Resolve `file_path` to a upath.UPath object
         """
         if str(self.file_path).endswith("/"):
             self.file_path = str(self.file_path)[:-1]
+        if "github" in str(self.file_path):
+            self.file_path = handle_github_url(url=str(self.file_path))
         return (
             upath.UPath(self.file_path).resolve()
             if self.file_path
             else pathlib.Path.cwd().resolve()
         )
 
 
@@ -162,21 +164,20 @@
 
     def render(self) -> RenderableType:
         """
         Render the Current File Info Bar
         """
         if self.file_info is None or not self.file_info.is_file:
             return Text("")
-        modify_time = self.file_info.last_modified.strftime("%b, %-d %Y %I:%M %p")
-        status_string = (
-            "🗄️️️  "
-            + self._convert_size(self.file_info.size)
-            + "   📅️  "
-            + modify_time
-            + "  💾  "
+        status_string = "🗄️️️  " + self._convert_size(self.file_info.size)
+        if self.file_info.last_modified is not None:
+            modify_time = self.file_info.last_modified.strftime("%b, %-d %Y %I:%M %p")
+            status_string += "  📅  " + modify_time
+        status_string += (
+            "  💾  "
             + self.file_info.file.name
             + "  📂  "
             + self.file_info.file.parent.name
         )
         if self.file_info.owner not in ["", None]:
             status_string += "  👤  " + self.file_info.owner
         if self.file_info.group.strip() not in ["", None]:
```

### Comparing `browsr-1.6.0/browsr/_cli.py` & `browsr-1.7.0/browsr/_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,17 +45,20 @@
 )
 def browsr(
     path: Optional[str],
     debug: bool,
     max_file_size: int,
 ) -> None:
     """
-    **`browsr`** is a file browser TUI (textual user interface) application. The application
-    allows you to visually browse through a directory (local or cloud) and display the
-    contents of its files
+    browsr 🗂️  a pleasant file explorer in your terminal
+
+    Navigate through directories and peek at files whether they're hosted locally,
+    in GitHub, AWS S3, Google Cloud Storage, or Azure Blob Storage. View code files
+    with syntax highlighting, format JSON files, render images, convert data files to navigable
+    datatables, and more.
 
     \f
 
     ![browsr](https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_utils.png)
 
     ## Installation
 
@@ -65,26 +68,46 @@
 
     ```shell
     pipx install "browsr[all]"
     ```
 
     ## Usage Examples
 
-    - Load your current working directory: **`browsr`**
-    - Load a specific directory: **`browsr /path/to/directory`**
-    - Load an S3 bucket: **`browsr s3://bucket-name`**
-    - Load a GCS bucket: **`browsr gs://bucket-name`**
+    - Load your current working directory
+        ```shell
+        browsr
+        ```
+    - Load a local directory
+        ```shell
+        browsr/path/to/directory
+        ```
+    - Load an S3 bucket
+        ```shell
+        browsr s3://bucket-name
+        ```
+    - Load a GCS bucket
+        ```shell
+        browsr gs://bucket-name
+        ```
+    - Load a GitHub repository
+        ```shell
+        browsr github://juftin:browsr
+        ```
+    - Load a GitHub repository branch
+        ```shell
+        browsr github://juftin:browsr@main
+        ```
 
     ## Key Bindings
-    - **`q`** - Quit the application
-    - **`f`** - Toggle the file tree sidebar
-    - **`t`** - Toggle the rich theme for code formatting
-    - **`n`** - Toggle line numbers for code formatting
-    - **`d`** - Toggle dark mode for the application
-    - **`x`** - Download the file from cloud storage
+    - **`Q`** - Quit the application
+    - **`F`** - Toggle the file tree sidebar
+    - **`T`** - Toggle the rich theme for code formatting
+    - **`N`** - Toggle line numbers for code formatting
+    - **`D`** - Toggle dark mode for the application
+    - **`X`** - Download the file from cloud storage
     """
     config = TextualAppContext(file_path=path, debug=debug, max_file_size=max_file_size)
     app = Browsr(config_object=config)
     app.run()
 
 
 if __name__ == "__main__":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `browsr-1.6.0/browsr/_config.py` & `browsr-1.7.0/browsr/_config.py`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/browsr/_tools.py` & `browsr-1.7.0/browsr/_tools.py`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/browsr/_utils.py` & `browsr-1.7.0/browsr/_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 Code Browsr Utility Functions
 """
 
 import datetime
 import os
 import pathlib
 from dataclasses import dataclass
-from typing import Any, BinaryIO, Dict, Union
+from typing import Any, BinaryIO, Dict, Optional, Union
 
 import fitz  # type: ignore[import]
+import requests
 import rich_pixels
 from fitz import Pixmap
 from PIL import Image
 from rich_pixels import Pixels
 from upath.implementations.cloud import CloudPath
 
+from browsr.universal_directory_tree import GitHubPath
+
 
 def _open_pdf_as_image(buf: BinaryIO) -> Image.Image:
     """
     Open a PDF file and return a PIL.Image object
     """
     doc = fitz.open(stream=buf.read(), filetype="pdf")
     pix: Pixmap = doc[0].get_pixmap()
     if pix.colorspace is None:
         mode = "L"
-    elif pix.colorspace.n == 1:  # PLR2004
+    elif pix.colorspace.n == 1:
         mode = "L" if pix.alpha == 0 else "LA"
-    elif pix.colorspace.n == 3:  # noqa PLR2004
+    elif pix.colorspace.n == 3:  # noqa: PLR2004
         mode = "RGB" if pix.alpha == 0 else "RGBA"
     else:
         mode = "CMYK"
     return Image.frombytes(size=(pix.width, pix.height), data=pix.samples, mode=mode)
 
 
 def open_image(document: pathlib.Path, screen_width: float) -> Pixels:
@@ -55,32 +58,31 @@
 class FileInfo:
     """
     File Information Object
     """
 
     file: pathlib.Path
     size: int
-    last_modified: datetime.datetime
+    last_modified: Optional[datetime.datetime]
     stat: Union[Dict[str, Any], os.stat_result]
     is_local: bool
     is_file: bool
     owner: str
     group: str
     is_cloudpath: bool
 
 
 def get_file_info(file_path: pathlib.Path) -> FileInfo:
     """
     Get File Information, Regardless of the FileSystem
     """
     stat = file_path.stat()
     is_file = file_path.is_file()
-    is_cloudpath = isinstance(file_path, CloudPath)
+    is_cloudpath = isinstance(file_path, (CloudPath, GitHubPath))
     if isinstance(stat, dict):
-        # raise ValueError(json.dumps(stat, indent=4))
         lower_dict = {key.lower(): value for key, value in stat.items()}
         file_size = lower_dict["size"]
         last_modified = lower_dict.get("lastmodified") or lower_dict.get("updated")
         if isinstance(last_modified, str):
             last_modified = datetime.datetime.fromisoformat(last_modified[:-1])
         return FileInfo(
             file=file_path,
@@ -121,7 +123,31 @@
         i = 1
         while True:
             new_file_stem = f"{file_path.stem} ({i})"
             new_file_path = file_path.with_stem(new_file_stem)
             if not new_file_path.exists():
                 return new_file_path
             i += 1
+
+
+def handle_github_url(url: str) -> str:
+    """
+    Handle GitHub URLs
+
+    GitHub URLs are handled by converting them to the raw URL.
+    """
+    if "github://" in url and "@" not in url:
+        _, user_password = url.split("github://")
+        org, repo = user_password.split(":")
+    elif "github://" in url and "@" in url:
+        return url
+    elif "github.com" in url and "https" in url:
+        _, url = url.split("://")
+        _, org, repo, *args = url.split("/")
+    resp = requests.get(
+        f"https://api.github.com/repos/{org}/{repo}",
+        headers={"Accept": "application/vnd.github.v3+json"},
+    )
+    resp.raise_for_status()
+    default_branch = resp.json()["default_branch"]
+    github_uri = f"github://{org}:{repo}@{default_branch}"
+    return github_uri
```

### Comparing `browsr-1.6.0/browsr/browsr.css` & `browsr-1.7.0/browsr/browsr.css`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/browsr/browsr.py` & `browsr-1.7.0/browsr/browsr.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from browsr._utils import (
     FileInfo,
     get_file_info,
     handle_duplicate_filenames,
     open_image,
 )
 from browsr._version import __application__
-from browsr.universal_directory_tree import UniversalDirectoryTree
+from browsr.universal_directory_tree import GitHubPath, UniversalDirectoryTree
 
 
 class Browsr(BrowsrTextualApp):
     """
     Textual code browser app.
     """
 
@@ -74,15 +74,15 @@
 
     def compose(self) -> Iterable[Widget]:
         """
         Compose our UI.
         """
         assert isinstance(self.config_object, TextualAppContext)
         file_path = self.config_object.path
-        if isinstance(file_path, CloudPath):
+        if isinstance(file_path, (CloudPath, GitHubPath)):
             self.bind("x", "download_file", description="Download File", show=True)
         if file_path.is_file():
             self.selected_file_path = file_path
             file_path = file_path.parent
         elif file_path.is_dir() and file_path.joinpath("README.md").exists():
             if TYPE_CHECKING:
                 assert isinstance(file_path, pathlib.Path)
@@ -179,15 +179,15 @@
         """
         Handle a File Size
         """
         file_size_mb = file_info.size / 1000 / 1000
         too_large = file_size_mb >= self.config_object.max_file_size  # type: ignore[union-attr]
         exception = (
             True
-            if not isinstance(file_info.file, CloudPath)
+            if not isinstance(file_info.file, (CloudPath, GitHubPath))
             and ".csv" in file_info.file.suffixes
             else False
         )
         if too_large is True and exception is not True:
             raise FileSizeError("File too large")
 
     def render_code_page(
@@ -318,29 +318,29 @@
         """
         Download the selected file.
         """
         if self.selected_file_path is None:
             return
         elif self.selected_file_path.is_dir():
             return
-        elif isinstance(self.selected_file_path, CloudPath):
+        elif isinstance(self.selected_file_path, (CloudPath, GitHubPath)):
             handled_download_path = self._get_download_file_name()
             with self.selected_file_path.open("rb") as file_handle:
                 with handled_download_path.open("wb") as download_handle:
                     shutil.copyfileobj(file_handle, download_handle)
 
     def action_download_file(self) -> None:
         """
         Download the selected file.
         """
         if self.selected_file_path is None:
             return
         elif self.selected_file_path.is_dir():
             return
-        elif isinstance(self.selected_file_path, CloudPath):
+        elif isinstance(self.selected_file_path, (CloudPath, GitHubPath)):
             handled_download_path = self._get_download_file_name()
             prompt_message: str = dedent(
                 f"""
                 ## File Download
 
                 **Are you sure you want to download that file?**
```

### Comparing `browsr-1.6.0/browsr/universal_directory_tree.py` & `browsr-1.7.0/browsr/universal_directory_tree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 """
 A universal directory tree widget for Textual.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import ClassVar, Iterable, Optional
+from typing import Any, ClassVar, Iterable, Optional
 
+import upath
 from textual.events import Mount
 from textual.reactive import var
 from textual.widgets import DirectoryTree
 from textual.widgets._tree import Tree, TreeNode
 from upath import UPath as Path
 
+upath.registry._registry.known_implementations[
+    "github"
+] = "browsr.universal_directory_tree.GitHubPath"
+
 
 @dataclass
 class DirEntry:
     """
     Attaches directory information to a node.
     """
 
@@ -139,7 +144,54 @@
                 path_name = str(path).replace("s3://", "").rstrip("/")
             node.add(
                 path_name,
                 data=DirEntry(path),  # type: ignore[arg-type]
                 allow_expand=path.is_dir(),
             )
         node.expand()
+
+
+class GitHubPath(upath.core.UPath):
+    """
+    GitHubPath
+
+    UPath implementation for GitHub to be compatible with
+    the Universal Directory Tree
+    """
+
+    @property
+    def path(self) -> str:
+        """
+        Paths get their leading slash stripped
+        """
+        return super().path.strip("/")
+
+    @property
+    def name(self) -> str:
+        """
+        Override the name for top level repo
+        """
+        if self.path == "":
+            org = self._accessor._fs.org
+            repo = self._accessor._fs.repo
+            sha = self._accessor._fs.sha
+            github_name = f"{org}:{repo}@{sha}"
+            return github_name
+        else:
+            return super().name
+
+    def __getattr__(self, item: str) -> Any:
+        """
+        Override the getattr method to allow for the name attribute override
+
+        This is necessary because the name attribute is not a property
+        of the UPath class
+        """
+        if item == "name":
+            github_name = (
+                f"{self._accessor._fs.org}:"
+                f"{self._accessor._fs.repo}"
+                f"@{self._accessor._fs.storage_options['sha']}"
+            )
+            return github_name
+        else:
+            return super().__getattr__(item)
```

### Comparing `browsr-1.6.0/docs/contributing.md` & `browsr-1.7.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/docs/gen_ref_pages.py` & `browsr-1.7.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/docs/index.md` & `browsr-1.7.0/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,22 @@
 </div>
 
 [![browsr Version](https://img.shields.io/pypi/v/browsr?color=blue&label=browsr)](https://github.com/juftin/browsr)
 [![PyPI](https://img.shields.io/pypi/pyversions/browsr)](https://pypi.python.org/pypi/browsr/)
 [![Testing Status](https://github.com/juftin/browsr/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/workflows/tests.yaml?query=branch%3Amain)
 [![GitHub License](https://img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://github.com/juftin/browsr/blob/main/LICENSE)
 
-**`browsr`** is a TUI (text-based user interface) file browser for your terminal.
-It's a simple way to browse your files and take a peek at their contents. Plus it
-works on local and remote file systems.
+**`browsr`** 🗂️ is a pleasant **file explorer** in your terminal. It's a command line **TUI**
+(text-based user interface) application that empowers you to browse the contents of local
+and remote filesystems with your keyboard or mouse.
+
+You can quickly navigate through directories and peek at files whether they're hosted **locally**,
+in **GitHub**, **AWS S3**, **Google Cloud Storage**, or **Azure Blob Storage**. View code files
+with syntax highlighting, format JSON files, render images, convert data files to navigable
+datatables, and more.
 
 <style>
   .grid-item {
     transition: all 0.5s ease;
   }
 
   .grid-item:hover {
@@ -69,39 +74,60 @@
     var expanded = document.querySelector('.expanded');
     expanded.onclick = function() {
       this.style.display = 'none';
     };
   </script>
 </body>
 
+<details>
+<summary>Screen Recording</summary>
+<video controls>
+  <source src="https://user-images.githubusercontent.com/49741340/238535232-459847af-a15c-4d9b-91ac-fab9958bc74f.mp4" type="video/mp4">
+  Your browser does not support the video tag.
+</video>
+</details>
+
 ## Installation
 
-The below command recommends [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx` installs the package in
-an isolated environment and makes it easy to uninstall. If you'd like to use `pip` instead, just replace `pipx`
+It's recommended to use [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx` installs the package in
+an isolated environment and makes it available everywhere. If you'd like to use `pip` instead, just replace `pipx`
 with `pip` in the below command.
 
 ```shell
 pipx install browsr
 ```
 
-## Extra Installation
+### Extra Installation
 
-If you're looking to use **`browsr`** on remote file systems, like AWS S3, you'll need to install the `remote` extra.
+If you're looking to use **`browsr`** on remote file systems, like GitHub or AWS S3, you'll need to install the `remote` extra.
 If you'd like to browse parquet files, you'll need to install the `parquet` extra. Or, even simpler,
 you can install the `all` extra to get all the extras.
 
 ```shell
 pipx install "browsr[all]"
 ```
 
 ## Usage
 
+Simply give **`browsr`** a path to a local or remote file / directory.
+[Check out the Documentation](https://juftin.com/browsr/) for more information
+about the file systems supported.
+
+### Local
+
 ```shell
 browsr ~/Downloads/
 ```
 
-Simply give **`browsr`** a path to a file/directory and it will open a browser window
-with a file browser. You can also give it a URL to a remote file system, like AWS S3.
+### GitHub
+
+```
+browsr github://juftin:browsr
+```
+
+### Cloud
 
 ```shell
-browsr s3://my-bucket/my-file.parquet
+browsr s3://my-bucket
 ```
+
+** _Currently AWS S3, Google Cloud Storage, and Azure Blob Storage are supported._
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -3,28 +3,35 @@
 [![browsr Version](https://img.shields.io/pypi/v/
 browsr?color=blue&label=browsr)](https://github.com/juftin/browsr) [![PyPI]
 (https://img.shields.io/pypi/pyversions/browsr)](https://pypi.python.org/pypi/
 browsr/) [![Testing Status](https://github.com/juftin/browsr/actions/workflows/
 tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/
 workflows/tests.yaml?query=branch%3Amain) [![GitHub License](https://
 img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://
-github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** is a TUI (text-based
-user interface) file browser for your terminal. It's a simple way to browse
-your files and take a peek at their contents. Plus it works on local and remote
-file systems.
+github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** ðï¸ is a pleasant
+**file explorer** in your terminal. It's a command line **TUI** (text-based
+user interface) application that empowers you to browse the contents of local
+and remote filesystems with your keyboard or mouse. You can quickly navigate
+through directories and peek at files whether they're hosted **locally**, in
+**GitHub**, **AWS S3**, **Google Cloud Storage**, or **Azure Blob Storage**.
+View code files with syntax highlighting, format JSON files, render images,
+convert data files to navigable datatables, and more.
 [Image 1]
 [Image 2]
 [Image 3]
 [Image 4]
 [Image]
-## Installation The below command recommends [pipx](https://pypa.github.io/
-pipx/) instead of pip. `pipx` installs the package in an isolated environment
-and makes it easy to uninstall. If you'd like to use `pip` instead, just
-replace `pipx` with `pip` in the below command. ```shell pipx install browsr
-``` ## Extra Installation If you're looking to use **`browsr`** on remote file
-systems, like AWS S3, you'll need to install the `remote` extra. If you'd like
-to browse parquet files, you'll need to install the `parquet` extra. Or, even
-simpler, you can install the `all` extra to get all the extras. ```shell pipx
-install "browsr[all]" ``` ## Usage ```shell browsr ~/Downloads/ ``` Simply give
-**`browsr`** a path to a file/directory and it will open a browser window with
-a file browser. You can also give it a URL to a remote file system, like AWS
-S3. ```shell browsr s3://my-bucket/my-file.parquet ```
+ Screen Recording   Your browser does not support the video tag.   ##
+Installation It's recommended to use [pipx](https://pypa.github.io/pipx/
+) instead of pip. `pipx` installs the package in an isolated environment and
+makes it available everywhere. If you'd like to use `pip` instead, just replace
+`pipx` with `pip` in the below command. ```shell pipx install browsr ``` ###
+Extra Installation If you're looking to use **`browsr`** on remote file
+systems, like GitHub or AWS S3, you'll need to install the `remote` extra. If
+you'd like to browse parquet files, you'll need to install the `parquet` extra.
+Or, even simpler, you can install the `all` extra to get all the extras.
+```shell pipx install "browsr[all]" ``` ## Usage Simply give **`browsr`** a
+path to a local or remote file / directory. [Check out the Documentation]
+(https://juftin.com/browsr/) for more information about the file systems
+supported. ### Local ```shell browsr ~/Downloads/ ``` ### GitHub ``` browsr
+github://juftin:browsr ``` ### Cloud ```shell browsr s3://my-bucket ``` **
+_Currently AWS S3, Google Cloud Storage, and Azure Blob Storage are supported._
```

### Comparing `browsr-1.6.0/docs/_static/browsr.png` & `browsr-1.7.0/docs/_static/browsr.png`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/docs/_static/browsr_no_label.png` & `browsr-1.7.0/docs/_static/browsr_no_label.png`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/docs/_static/screenshot_datatable.png` & `browsr-1.7.0/docs/_static/screenshot_datatable.png`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/docs/_static/screenshot_markdown.png` & `browsr-1.7.0/docs/_static/screenshot_markdown.png`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/docs/_static/screenshot_mona_lisa.png` & `browsr-1.7.0/docs/_static/screenshot_mona_lisa.png`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/docs/_static/screenshot_utils.png` & `browsr-1.7.0/docs/_static/screenshot_utils.png`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/requirements/requirements-dev.txt` & `browsr-1.7.0/requirements/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1282,22 +1282,27 @@
 pytest==7.3.1 \
     --hash=sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362 \
     --hash=sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3
     # via
     #   -r requirements.in
     #   pytest-cov
     #   pytest-mock
+    #   pytest-vcr
 pytest-cov==4.0.0 \
     --hash=sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b \
     --hash=sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470
     # via -r requirements.in
 pytest-mock==3.10.0 \
     --hash=sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b \
     --hash=sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f
     # via -r requirements.in
+pytest-vcr==1.0.2 \
+    --hash=sha256:23ee51b75abbcc43d926272773aae4f39f93aceb75ed56852d0bf618f92e1896 \
+    --hash=sha256:2f316e0539399bea0296e8b8401145c62b6f85e9066af7e57b6151481b0d6d9c
+    # via -r requirements.in
 python-dateutil==2.8.2 \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
     # via
     #   adal
     #   botocore
     #   ghp-import
@@ -1347,14 +1352,15 @@
     --hash=sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f \
     --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
     --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
     # via
     #   mkdocs
     #   pymdown-extensions
     #   pyyaml-env-tag
+    #   vcrpy
 pyyaml-env-tag==0.1 \
     --hash=sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb \
     --hash=sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069
     # via mkdocs
 regex==2023.5.5 \
     --hash=sha256:02f4541550459c08fdd6f97aa4e24c6f1932eec780d58a2faa2068253df7d6ff \
     --hash=sha256:0a69cf0c00c4d4a929c6c7717fd918414cab0d6132a49a6d8fc3ded1988ed2ea \
@@ -1511,14 +1517,15 @@
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via
     #   azure-core
     #   azure-identity
     #   google-auth
     #   isodate
     #   python-dateutil
+    #   vcrpy
 textual[dev]==0.24.1 \
     --hash=sha256:4c7e1f4ed12b9615c63fa3eb7cb9df68d29e0ae5b2352997958cd7ee5533f926 \
     --hash=sha256:a7deb7ac5a1502424c754fe165ae13cb3890e47ddc514d3f089cb2984c336d1d
     # via -r requirements.in
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
@@ -1551,14 +1558,18 @@
     # via -r requirements.in
 urllib3==1.26.15 \
     --hash=sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305 \
     --hash=sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42
     # via
     #   botocore
     #   requests
+vcrpy==4.2.1 \
+    --hash=sha256:7cd3e81a2c492e01c281f180bcc2a86b520b173d2b656cb5d89d99475423e013 \
+    --hash=sha256:efac3e2e0b2af7686f83a266518180af7a048619b2f696e7bad9520f5e2eac09
+    # via pytest-vcr
 watchdog==3.0.0 \
     --hash=sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a \
     --hash=sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100 \
     --hash=sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8 \
     --hash=sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc \
     --hash=sha256:2b57a1e730af3156d13b7fdddfc23dea6487fceca29fc75c5a868beed29177ae \
     --hash=sha256:336adfc6f5cc4e037d52db31194f7581ff744b67382eb6021c868322e32eef41 \
@@ -1660,15 +1671,17 @@
     --hash=sha256:e20076a211cd6f9b44a6be58f7eeafa7ab5720eb796975d0c03f05b47d89eb90 \
     --hash=sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29 \
     --hash=sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6 \
     --hash=sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034 \
     --hash=sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09 \
     --hash=sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559 \
     --hash=sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639
-    # via aiobotocore
+    # via
+    #   aiobotocore
+    #   vcrpy
 yarl==1.9.2 \
     --hash=sha256:04ab9d4b9f587c06d801c2abfe9317b77cdf996c65a90d5e84ecc45010823571 \
     --hash=sha256:066c163aec9d3d073dc9ffe5dd3ad05069bcb03fcaab8d221290ba99f9f69ee3 \
     --hash=sha256:13414591ff516e04fcdee8dc051c13fd3db13b673c7a4cb1350e6b2ad9639ad3 \
     --hash=sha256:149ddea5abf329752ea5051b61bd6c1d979e13fbf122d3a1f9f0c8be6cb6f63c \
     --hash=sha256:159d81f22d7a43e6eabc36d7194cb53f2f15f498dbbfa8edc8a3239350f59fe7 \
     --hash=sha256:1b1bba902cba32cdec51fca038fd53f8beee88b77efc373968d1ed021024cc04 \
@@ -1736,15 +1749,17 @@
     --hash=sha256:e65610c5792870d45d7b68c677681376fcf9cc1c289f23e8e8b39c1485384185 \
     --hash=sha256:e9fdc7ac0d42bc3ea78818557fab03af6181e076a2944f43c38684b4b6bed8e3 \
     --hash=sha256:ee4afac41415d52d53a9833ebae7e32b344be72835bbb589018c9e938045a560 \
     --hash=sha256:f364d3480bffd3aa566e886587eaca7c8c04d74f6e8933f3f2c996b7f09bee1b \
     --hash=sha256:f3b078dbe227f79be488ffcfc7a9edb3409d018e0952cf13f15fd6512847f3f7 \
     --hash=sha256:f4e2d08f07a3d7d3e12549052eb5ad3eab1c349c53ac51c209a0e5991bbada78 \
     --hash=sha256:f7a3d8146575e08c29ed1cd287068e6d02f1c7bdff8970db96683b9591b86ee7
-    # via aiohttp
+    # via
+    #   aiohttp
+    #   vcrpy
 zipp==3.15.0 \
     --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
     --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
     # via importlib-metadata
 
 # WARNING: The following packages were not pinned, but pip requires them to be
 # pinned when the requirements file includes hashes. Consider using the --allow-unsafe flag.
```

### Comparing `browsr-1.6.0/requirements/requirements-prod.txt` & `browsr-1.7.0/requirements/requirements-prod.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/tests/conftest.py` & `browsr-1.7.0/tests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Pytest Fixtures Shared Across all Unit Tests
 """
 
 import pathlib
+from typing import Any, Dict, List
 
 import pytest
 from click.testing import CliRunner
 
-from browsr import Browsr
-from browsr._base import TextualAppContext
+from browsr.universal_directory_tree import GitHubPath
 
 
 @pytest.fixture
 def runner() -> CliRunner:
     """
     Return a CliRunner object
     """
@@ -32,16 +32,34 @@
     """
     Return the path to the screenshot directory
     """
     return repo_dir / "tests" / "screenshots"
 
 
 @pytest.fixture
-def app(repo_dir: pathlib.Path) -> Browsr:
+def github_release_path() -> GitHubPath:
     """
-    Textual Screenshotting Tests
+    Return the path to the Github Release
     """
-    context = TextualAppContext(
-        file_path=str(repo_dir),
-    )
-    app = Browsr(config_object=context)
-    return app
+    release = "v1.6.0"
+    uri = f"github://juftin:browsr@{release}"
+    return GitHubPath(uri)
+
+
+@pytest.fixture(scope="module")
+def vcr_config() -> Dict[str, List[Any]]:
+    """
+    VCR Cassette Privacy Enforcer
+
+    This fixture ensures the API Credentials are obfuscated
+
+    Returns
+    -------
+    Dict[str, list]:
+    """
+    return {
+        "filter_headers": [("authorization", "XXXXXXXXXX")],
+        "filter_query_parameters": [("user", "XXXXXXXXXX"), ("token", "XXXXXXXXXX")],
+    }
+
+
+cassette = pytest.mark.vcr(scope="module")
```

### Comparing `browsr-1.6.0/.gitignore` & `browsr-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/LICENSE` & `browsr-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browsr-1.6.0/README.md` & `browsr-1.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,62 +8,87 @@
 </div>
 
 [![browsr Version](https://img.shields.io/pypi/v/browsr?color=blue&label=browsr)](https://github.com/juftin/browsr)
 [![PyPI](https://img.shields.io/pypi/pyversions/browsr)](https://pypi.python.org/pypi/browsr/)
 [![Testing Status](https://github.com/juftin/browsr/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/workflows/tests.yaml?query=branch%3Amain)
 [![GitHub License](https://img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://github.com/juftin/browsr/blob/main/LICENSE)
 
-**`browsr`** is a TUI (text-based user interface) file browser for your terminal.
-It's a simple way to browse your files and take a peek at their contents. Plus it
-works on local and remote file systems.
+**`browsr`** 🗂️ is a pleasant **file explorer** in your terminal. It's a command line **TUI**
+(text-based user interface) application that empowers you to browse the contents of local
+and remote filesystems with your keyboard or mouse.
+
+You can quickly navigate through directories and peek at files whether they're hosted **locally**,
+in **GitHub**, **AWS S3**, **Google Cloud Storage**, or **Azure Blob Storage**. View code files
+with syntax highlighting, format JSON files, render images, convert data files to navigable
+datatables, and more.
 
-<details open></summary></summary>
+![](https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_utils.png)
+
+<details>
+<summary>Screenshots</summary>
 
 <body>
-<div style="display: grid; grid-template-columns: repeat(2, 1fr); grid-gap: 10px;">
-    <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_utils.png" alt="Image 1">
+<div>
     <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_datatable.png" alt="Image 2">
     <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_mona_lisa.png" alt="Image 3">
     <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_markdown.png" alt="Image 4">
 </div>
 </body>
 
 </details>
 
+<details>
+<summary>Screen Recording</summary>
+
+https://user-images.githubusercontent.com/49741340/238535232-459847af-a15c-4d9b-91ac-fab9958bc74f.mp4
+
+</details>
+
 ## Installation
 
-The below command recommends [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx` installs the package in
-an isolated environment and makes it easy to uninstall. If you'd like to use `pip` instead, just replace `pipx`
+It's recommended to use [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx` installs the package in
+an isolated environment and makes it available everywhere. If you'd like to use `pip` instead, just replace `pipx`
 with `pip` in the below command.
 
 ```shell
 pipx install browsr
 ```
 
-## Extra Installation
+### Extra Installation
 
-If you're looking to use **`browsr`** on remote file systems, like AWS S3, you'll need to install the `remote` extra.
+If you're looking to use **`browsr`** on remote file systems, like GitHub or AWS S3, you'll need to install the `remote` extra.
 If you'd like to browse parquet files, you'll need to install the `parquet` extra. Or, even simpler,
 you can install the `all` extra to get all the extras.
 
 ```shell
 pipx install "browsr[all]"
 ```
 
 ## Usage
 
+Simply give **`browsr`** a path to a local or remote file / directory.
+[Check out the Documentation](https://juftin.com/browsr/) for more information
+about the file systems supported.
+
+### Local
+
 ```shell
 browsr ~/Downloads/
 ```
 
-Simply give **`browsr`** a path to a file/directory and it will open a browser window
-with a file browser. You can also give it a URL to a remote file system, like AWS S3.
+### GitHub
+
+```
+browsr github://juftin:browsr
+```
+
+### Cloud
 
 ```shell
-browsr s3://my-bucket/my-file.parquet
+browsr s3://my-bucket
 ```
 
-### [Check out the Documentation](https://juftin.com/browsr/) for more
+\*\* _Currently AWS S3, Google Cloud Storage, and Azure Blob Storage are supported._
 
 ## License
 
 **`browsr`** is distributed under the terms of the [MIT license](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -3,26 +3,35 @@
 [![browsr Version](https://img.shields.io/pypi/v/
 browsr?color=blue&label=browsr)](https://github.com/juftin/browsr) [![PyPI]
 (https://img.shields.io/pypi/pyversions/browsr)](https://pypi.python.org/pypi/
 browsr/) [![Testing Status](https://github.com/juftin/browsr/actions/workflows/
 tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/
 workflows/tests.yaml?query=branch%3Amain) [![GitHub License](https://
 img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://
-github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** is a TUI (text-based
-user interface) file browser for your terminal. It's a simple way to browse
-your files and take a peek at their contents. Plus it works on local and remote
-file systems.
-[Image 1] [Image 2] [Image 3] [Image 4]
- ## Installation The below command recommends [pipx](https://pypa.github.io/
-pipx/) instead of pip. `pipx` installs the package in an isolated environment
-and makes it easy to uninstall. If you'd like to use `pip` instead, just
-replace `pipx` with `pip` in the below command. ```shell pipx install browsr
-``` ## Extra Installation If you're looking to use **`browsr`** on remote file
-systems, like AWS S3, you'll need to install the `remote` extra. If you'd like
-to browse parquet files, you'll need to install the `parquet` extra. Or, even
-simpler, you can install the `all` extra to get all the extras. ```shell pipx
-install "browsr[all]" ``` ## Usage ```shell browsr ~/Downloads/ ``` Simply give
-**`browsr`** a path to a file/directory and it will open a browser window with
-a file browser. You can also give it a URL to a remote file system, like AWS
-S3. ```shell browsr s3://my-bucket/my-file.parquet ``` ### [Check out the
-Documentation](https://juftin.com/browsr/) for more ## License **`browsr`** is
+github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** ðï¸ is a pleasant
+**file explorer** in your terminal. It's a command line **TUI** (text-based
+user interface) application that empowers you to browse the contents of local
+and remote filesystems with your keyboard or mouse. You can quickly navigate
+through directories and peek at files whether they're hosted **locally**, in
+**GitHub**, **AWS S3**, **Google Cloud Storage**, or **Azure Blob Storage**.
+View code files with syntax highlighting, format JSON files, render images,
+convert data files to navigable datatables, and more. ![](https://
+raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_utils.png)
+Screenshots
+[Image 2] [Image 3] [Image 4]
+  Screen Recording https://user-images.githubusercontent.com/49741340/
+238535232-459847af-a15c-4d9b-91ac-fab9958bc74f.mp4  ## Installation It's
+recommended to use [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx`
+installs the package in an isolated environment and makes it available
+everywhere. If you'd like to use `pip` instead, just replace `pipx` with `pip`
+in the below command. ```shell pipx install browsr ``` ### Extra Installation
+If you're looking to use **`browsr`** on remote file systems, like GitHub or
+AWS S3, you'll need to install the `remote` extra. If you'd like to browse
+parquet files, you'll need to install the `parquet` extra. Or, even simpler,
+you can install the `all` extra to get all the extras. ```shell pipx install
+"browsr[all]" ``` ## Usage Simply give **`browsr`** a path to a local or remote
+file / directory. [Check out the Documentation](https://juftin.com/browsr/) for
+more information about the file systems supported. ### Local ```shell browsr ~/
+Downloads/ ``` ### GitHub ``` browsr github://juftin:browsr ``` ### Cloud
+```shell browsr s3://my-bucket ``` \*\* _Currently AWS S3, Google Cloud
+Storage, and Azure Blob Storage are supported._ ## License **`browsr`** is
 distributed under the terms of the [MIT license](LICENSE).
```

### Comparing `browsr-1.6.0/pyproject.toml` & `browsr-1.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 parallel = true
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest~=7.3.1",
   "pytest-cov~=4.0.0",
   "pytest-mock~=3.10.0",
+  "pytest-vcr~=1.0.2",
   "mkdocs~=1.4.2",
   "mkdocs-material~=9.1.6",
   "mkdocs-click~=0.8.0",
   "mkdocstrings[python]~=0.21.2",
   "mkdocs-gen-files~=0.4.0",
   "mkdocs-literate-nav~=0.6.0",
   "mkdocs-section-index~=0.3.5",
```

### Comparing `browsr-1.6.0/PKG-INFO` & `browsr-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browsr
-Version: 1.6.0
+Version: 1.7.0
 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme
 Project-URL: Issues, https://github.com/juftin/browsr/issues
 Project-URL: Source, https://github.com/juftin/browsr
 Author-email: Justin Flannery <justin.flannery@juftin.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -53,62 +53,87 @@
 </div>
 
 [![browsr Version](https://img.shields.io/pypi/v/browsr?color=blue&label=browsr)](https://github.com/juftin/browsr)
 [![PyPI](https://img.shields.io/pypi/pyversions/browsr)](https://pypi.python.org/pypi/browsr/)
 [![Testing Status](https://github.com/juftin/browsr/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/workflows/tests.yaml?query=branch%3Amain)
 [![GitHub License](https://img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://github.com/juftin/browsr/blob/main/LICENSE)
 
-**`browsr`** is a TUI (text-based user interface) file browser for your terminal.
-It's a simple way to browse your files and take a peek at their contents. Plus it
-works on local and remote file systems.
+**`browsr`** 🗂️ is a pleasant **file explorer** in your terminal. It's a command line **TUI**
+(text-based user interface) application that empowers you to browse the contents of local
+and remote filesystems with your keyboard or mouse.
+
+You can quickly navigate through directories and peek at files whether they're hosted **locally**,
+in **GitHub**, **AWS S3**, **Google Cloud Storage**, or **Azure Blob Storage**. View code files
+with syntax highlighting, format JSON files, render images, convert data files to navigable
+datatables, and more.
 
-<details open></summary></summary>
+![](https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_utils.png)
+
+<details>
+<summary>Screenshots</summary>
 
 <body>
-<div style="display: grid; grid-template-columns: repeat(2, 1fr); grid-gap: 10px;">
-    <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_utils.png" alt="Image 1">
+<div>
     <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_datatable.png" alt="Image 2">
     <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_mona_lisa.png" alt="Image 3">
     <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_markdown.png" alt="Image 4">
 </div>
 </body>
 
 </details>
 
+<details>
+<summary>Screen Recording</summary>
+
+https://user-images.githubusercontent.com/49741340/238535232-459847af-a15c-4d9b-91ac-fab9958bc74f.mp4
+
+</details>
+
 ## Installation
 
-The below command recommends [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx` installs the package in
-an isolated environment and makes it easy to uninstall. If you'd like to use `pip` instead, just replace `pipx`
+It's recommended to use [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx` installs the package in
+an isolated environment and makes it available everywhere. If you'd like to use `pip` instead, just replace `pipx`
 with `pip` in the below command.
 
 ```shell
 pipx install browsr
 ```
 
-## Extra Installation
+### Extra Installation
 
-If you're looking to use **`browsr`** on remote file systems, like AWS S3, you'll need to install the `remote` extra.
+If you're looking to use **`browsr`** on remote file systems, like GitHub or AWS S3, you'll need to install the `remote` extra.
 If you'd like to browse parquet files, you'll need to install the `parquet` extra. Or, even simpler,
 you can install the `all` extra to get all the extras.
 
 ```shell
 pipx install "browsr[all]"
 ```
 
 ## Usage
 
+Simply give **`browsr`** a path to a local or remote file / directory.
+[Check out the Documentation](https://juftin.com/browsr/) for more information
+about the file systems supported.
+
+### Local
+
 ```shell
 browsr ~/Downloads/
 ```
 
-Simply give **`browsr`** a path to a file/directory and it will open a browser window
-with a file browser. You can also give it a URL to a remote file system, like AWS S3.
+### GitHub
+
+```
+browsr github://juftin:browsr
+```
+
+### Cloud
 
 ```shell
-browsr s3://my-bucket/my-file.parquet
+browsr s3://my-bucket
 ```
 
-### [Check out the Documentation](https://juftin.com/browsr/) for more
+\*\* _Currently AWS S3, Google Cloud Storage, and Azure Blob Storage are supported._
 
 ## License
 
 **`browsr`** is distributed under the terms of the [MIT license](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: browsr Version: 1.6.0 Summary: TUI File Browser App
+Metadata-Version: 2.1 Name: browsr Version: 1.7.0 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme Project-
 URL: Issues, https://github.com/juftin/browsr/issues Project-URL: Source,
 https://github.com/juftin/browsr Author-email: Justin Flannery
 flannery@juftin.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -25,26 +25,35 @@
 [![browsr Version](https://img.shields.io/pypi/v/
 browsr?color=blue&label=browsr)](https://github.com/juftin/browsr) [![PyPI]
 (https://img.shields.io/pypi/pyversions/browsr)](https://pypi.python.org/pypi/
 browsr/) [![Testing Status](https://github.com/juftin/browsr/actions/workflows/
 tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/
 workflows/tests.yaml?query=branch%3Amain) [![GitHub License](https://
 img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://
-github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** is a TUI (text-based
-user interface) file browser for your terminal. It's a simple way to browse
-your files and take a peek at their contents. Plus it works on local and remote
-file systems.
-[Image 1] [Image 2] [Image 3] [Image 4]
- ## Installation The below command recommends [pipx](https://pypa.github.io/
-pipx/) instead of pip. `pipx` installs the package in an isolated environment
-and makes it easy to uninstall. If you'd like to use `pip` instead, just
-replace `pipx` with `pip` in the below command. ```shell pipx install browsr
-``` ## Extra Installation If you're looking to use **`browsr`** on remote file
-systems, like AWS S3, you'll need to install the `remote` extra. If you'd like
-to browse parquet files, you'll need to install the `parquet` extra. Or, even
-simpler, you can install the `all` extra to get all the extras. ```shell pipx
-install "browsr[all]" ``` ## Usage ```shell browsr ~/Downloads/ ``` Simply give
-**`browsr`** a path to a file/directory and it will open a browser window with
-a file browser. You can also give it a URL to a remote file system, like AWS
-S3. ```shell browsr s3://my-bucket/my-file.parquet ``` ### [Check out the
-Documentation](https://juftin.com/browsr/) for more ## License **`browsr`** is
+github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** ðï¸ is a pleasant
+**file explorer** in your terminal. It's a command line **TUI** (text-based
+user interface) application that empowers you to browse the contents of local
+and remote filesystems with your keyboard or mouse. You can quickly navigate
+through directories and peek at files whether they're hosted **locally**, in
+**GitHub**, **AWS S3**, **Google Cloud Storage**, or **Azure Blob Storage**.
+View code files with syntax highlighting, format JSON files, render images,
+convert data files to navigable datatables, and more. ![](https://
+raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_utils.png)
+Screenshots
+[Image 2] [Image 3] [Image 4]
+  Screen Recording https://user-images.githubusercontent.com/49741340/
+238535232-459847af-a15c-4d9b-91ac-fab9958bc74f.mp4  ## Installation It's
+recommended to use [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx`
+installs the package in an isolated environment and makes it available
+everywhere. If you'd like to use `pip` instead, just replace `pipx` with `pip`
+in the below command. ```shell pipx install browsr ``` ### Extra Installation
+If you're looking to use **`browsr`** on remote file systems, like GitHub or
+AWS S3, you'll need to install the `remote` extra. If you'd like to browse
+parquet files, you'll need to install the `parquet` extra. Or, even simpler,
+you can install the `all` extra to get all the extras. ```shell pipx install
+"browsr[all]" ``` ## Usage Simply give **`browsr`** a path to a local or remote
+file / directory. [Check out the Documentation](https://juftin.com/browsr/) for
+more information about the file systems supported. ### Local ```shell browsr ~/
+Downloads/ ``` ### GitHub ``` browsr github://juftin:browsr ``` ### Cloud
+```shell browsr s3://my-bucket ``` \*\* _Currently AWS S3, Google Cloud
+Storage, and Azure Blob Storage are supported._ ## License **`browsr`** is
 distributed under the terms of the [MIT license](LICENSE).
```

