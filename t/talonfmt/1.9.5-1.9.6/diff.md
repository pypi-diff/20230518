# Comparing `tmp/talonfmt-1.9.5.tar.gz` & `tmp/talonfmt-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talonfmt-1.9.5.tar", max compression
+gzip compressed data, was "talonfmt-1.9.6.tar", last modified: Thu May 18 12:11:12 2023, max compression
```

## Comparing `talonfmt-1.9.5.tar` & `talonfmt-1.9.6.tar`

### file list

```diff
@@ -1,10 +1,24 @@
--rw-r--r--   0        0        0     1066 2023-03-09 22:16:58.151301 talonfmt-1.9.5/LICENSE
--rw-r--r--   0        0        0      444 2023-03-09 22:16:58.151395 talonfmt-1.9.5/README.md
--rw-r--r--   0        0        0     2014 2023-03-14 01:18:34.958455 talonfmt-1.9.5/pyproject.toml
--rw-r--r--   0        0        0     5441 2023-03-14 01:15:39.334842 talonfmt-1.9.5/talonfmt/__init__.py
--rw-r--r--   0        0        0     1282 2023-03-09 22:16:58.151933 talonfmt-1.9.5/talonfmt/assert_equivalent.py
--rw-r--r--   0        0        0     5209 2023-03-09 22:16:58.151996 talonfmt-1.9.5/talonfmt/cli.py
--rw-r--r--   0        0        0      909 2023-03-09 22:16:58.152041 talonfmt-1.9.5/talonfmt/editorconfig.py
--rw-r--r--   0        0        0    22315 2023-03-09 22:16:58.152137 talonfmt-1.9.5/talonfmt/formatter.py
--rw-r--r--   0        0        0        0 2023-03-09 22:16:58.152162 talonfmt-1.9.5/talonfmt/py.typed
--rw-r--r--   0        0        0     1550 1970-01-01 00:00:00.000000 talonfmt-1.9.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:12.725077 talonfmt-1.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 12:10:53.000000 talonfmt-1.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-18 12:11:12.725077 talonfmt-1.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-18 12:10:53.000000 talonfmt-1.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-18 12:10:53.000000 talonfmt-1.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:11:12.725077 talonfmt-1.9.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:12.725077 talonfmt-1.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:12.725077 talonfmt-1.9.6/src/talonfmt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-18 12:10:53.000000 talonfmt-1.9.6/src/talonfmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 12:10:53.000000 talonfmt-1.9.6/src/talonfmt/assert_equivalent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-18 12:10:53.000000 talonfmt-1.9.6/src/talonfmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-18 12:10:53.000000 talonfmt-1.9.6/src/talonfmt/editorconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-05-18 12:10:53.000000 talonfmt-1.9.6/src/talonfmt/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:12.725077 talonfmt-1.9.6/src/talonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 12:11:12.000000 talonfmt-1.9.6/src/talonfmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:11:12.725077 talonfmt-1.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-18 12:10:53.000000 talonfmt-1.9.6/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-18 12:10:53.000000 talonfmt-1.9.6/tests/test_smart1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-18 12:10:53.000000 talonfmt-1.9.6/tests/test_smart80.py
```

### Comparing `talonfmt-1.9.5/LICENSE` & `talonfmt-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `talonfmt-1.9.5/pyproject.toml` & `talonfmt-1.9.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,84 @@
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["setuptools>=45"]
+build-backend = "setuptools.build_meta"
 
-[tool.poetry]
+[project]
 name = "talonfmt"
-version = "1.9.5"
+version = "1.9.6"
 description = "A code formatter for Talon files"
-license = "MIT"
-authors = ["Wen Kokke <wenkokke@users.noreply.github.com>"]
+license = { file = 'LICENSE' }
+authors = [{ name = "Wen Kokke", email = "wenkokke@users.noreply.github.com" }]
 readme = "README.md"
-repository = "https://github.com/wenkokke/talonfmt"
 keywords = ["talon", "formatter"]
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Topic :: Software Development :: Compilers",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+]
+requires-python = ">=3.9.8,<3.12"
+dependencies = [
+  "click >=8.1.3,<9",
+  "dataclasses_json >=0.5.7,<0.6",
+  "doc_printer >=0.13.1,<0.14",
+  "editorconfig >=0.12.3,<0.13",
+  "tree_sitter_talon >=1007.3.2.0,<3!2",
 ]
 
-[tool.poetry.dependencies]
-python = "^3.9.8"
-click = "^8.1.3"
-bumpver = { version = "*", optional = true }
-doc-printer = "^0.13.1"
-editorconfig = "^0.12.3"
-pytest = { version = "^7.1.2", optional = true }
-pytest-benchmark = { version = ">=3.4.1,<5.0.0", optional = true }
-pytest-golden = { version = "^0.2.2", optional = true }
-tree-sitter-talon = "^1007.3.2.0"
-# Prevent Poetry 1.3 from removing setuptools
-setuptools = "*"
+[project.optional-dependencies]
+mypy = ["types_setuptools"]
+test = [
+  "bumpver",
+  "mypy >=1.1.1,<2",
+  "pytest >=7.1.2,<8",
+  "pytest_golden >=0.2.2,<0.3",
+  "pytest_benchmark >=3.4.1,<5.0.0"
+]
 
-[tool.poetry.extras]
-test = ["bumpver", "pytest", "pytest-benchmark", "pytest-golden"]
+[project.scripts]
+talondoc = "talonfmt.cli:cli"
 
-[tool.poetry.scripts]
-talonfmt = "talonfmt.cli:cli"
+[tool.bumpver]
+current_version = "1.9.6"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message = "Bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = true
 
-[tool.pytest.ini_options]
-enable_assertion_pass_hook = true
-filterwarnings = ["ignore::DeprecationWarning:.*:"]
-addopts = "--ignore=tests/data"
-testpaths = ["tests"]
+[tool.bumpver.file_patterns]
+"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
+"src/talonfmt/__init__.py" = ['__version__: str = "{version}"']
 
 [tool.mypy]
 python_version = 3.9
 namespace_packages = true
 explicit_package_bases = true
 ignore_missing_imports = true
 warn_redundant_casts = true
 warn_unused_configs = true
 
-[tool.bumpver]
-current_version = "1.9.5"
-version_pattern = "MAJOR.MINOR.PATCH"
-commit_message = "Bump version {old_version} -> {new_version}"
-commit = true
-tag = true
-push = true
+[tool.pytest.ini_options]
+enable_assertion_pass_hook = true
+filterwarnings = ["ignore::DeprecationWarning:.*:"]
+addopts = "--ignore=tests/data"
+testpaths = ["tests"]
 
-[tool.bumpver.file_patterns]
-"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"talonfmt/__init__.py" = ['__version__: str = "{version}"']
+[tool.setuptools.packages.find]
+where = ["src"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
+envlist = py39, py310, py311
 isolated_build = true
-envlist = py39,py310,py311
-
-[gh-actions]
-python =
-  3.9: py39
-  3.10: py310
-  3.11: py311
 
 [testenv]
-commands =
-    bumpver update --patch --dry --no-fetch
-    pytest --benchmark-disable -x
 extras =
-    test
+  test
+commands =
+  {envpython} -m bumpver update --patch --dry --no-fetch
+  {envpython} -m pytest tests --benchmark-disable -x
 """
```

### Comparing `talonfmt-1.9.5/talonfmt/__init__.py` & `talonfmt-1.9.6/src/talonfmt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from doc_printer import DocRenderer, SimpleDocRenderer, SimpleLayout, SmartDocRenderer
 from tree_sitter_talon import Node, parse
 
 from .editorconfig import get_indent_size, get_max_line_length
 from .formatter import EmptyMatchContext, TalonFormatter
 
-__version__: str = "1.9.5"
+__version__: str = "1.9.6"
 
 
 def talonfmt(
     contents: Union[str, bytes, Node],
     *,
     filename: Optional[str] = None,
     encoding: str = "utf-8",
```

### Comparing `talonfmt-1.9.5/talonfmt/assert_equivalent.py` & `talonfmt-1.9.6/src/talonfmt/assert_equivalent.py`

 * *Files identical despite different names*

### Comparing `talonfmt-1.9.5/talonfmt/cli.py` & `talonfmt-1.9.6/src/talonfmt/cli.py`

 * *Files identical despite different names*

### Comparing `talonfmt-1.9.5/talonfmt/editorconfig.py` & `talonfmt-1.9.6/src/talonfmt/editorconfig.py`

 * *Files identical despite different names*

### Comparing `talonfmt-1.9.5/talonfmt/formatter.py` & `talonfmt-1.9.6/src/talonfmt/formatter.py`

 * *Files identical despite different names*

