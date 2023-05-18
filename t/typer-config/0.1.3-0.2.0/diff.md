# Comparing `tmp/typer_config-0.1.3.tar.gz` & `tmp/typer_config-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_config-0.1.3.tar", max compression
+gzip compressed data, was "typer_config-0.2.0.tar", max compression
```

## Comparing `typer_config-0.1.3.tar` & `typer_config-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-15 03:20:33.887810 typer_config-0.1.3/LICENSE
--rw-r--r--   0        0        0     1044 2023-05-15 03:20:33.887810 typer_config-0.1.3/README.md
--rw-r--r--   0        0        0     2150 2023-05-15 03:20:33.887810 typer_config-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1621 2023-05-15 03:20:33.887810 typer_config-0.1.3/typer_config/__init__.py
--rw-r--r--   0        0        0     1089 2023-05-15 03:20:33.887810 typer_config-0.1.3/typer_config/__typing.py
--rw-r--r--   0        0        0     3758 2023-05-15 03:20:33.887810 typer_config-0.1.3/typer_config/loaders.py
--rw-r--r--   0        0        0     2936 1970-01-01 00:00:00.000000 typer_config-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-16 04:06:27.574721 typer_config-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1838 2023-05-16 04:34:58.786785 typer_config-0.2.0/README.md
+-rw-r--r--   0        0        0     2454 2023-05-18 00:01:41.974428 typer_config-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3945 2023-05-17 23:52:39.623396 typer_config-0.2.0/typer_config/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-16 04:06:27.578055 typer_config-0.2.0/typer_config/__typing.py
+-rw-r--r--   0        0        0     4560 2023-05-17 23:52:39.623396 typer_config-0.2.0/typer_config/loaders.py
+-rw-r--r--   0        0        0     3841 1970-01-01 00:00:00.000000 typer_config-0.2.0/PKG-INFO
```

### Comparing `typer_config-0.1.3/LICENSE` & `typer_config-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.3/pyproject.toml` & `typer_config-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-config"
-version = "0.1.3"
+version = "0.2.0"
 description = "Utilities for working with configuration files in typer CLIs. "
 authors = ["Matt Anderson <matt@manderscience.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "typer_config"}]
 repository = "https://github.com/maxb2/typer-config"
 documentation = "https://maxb2.github.io/typer-config/"
@@ -13,14 +13,15 @@
         "typer",
         "config",
         "configuration",
         "configuration-file",
         "yaml",
         "toml",
         "json",
+        "dotenv",
         "cli"
     ]
 classifiers = [
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
@@ -40,32 +41,45 @@
     ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typer = "^0"
 toml = {version = "^0.10.2", optional = true}
 pyyaml = {version = "^6.0", optional = true}
+python-dotenv = {version = "*", optional = true}
 
 [tool.poetry.extras]
+python-dotenv = ["python-dotenv"]
 toml = ["toml"]
 yaml = ["pyyaml"]
-all = ["toml", "pyyaml"]
+all = ["toml", "pyyaml", "python-dotenv"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.263"
 pylint = "^2.17.3"
 black = "^23.3.0"
 isort = "^5.12.0"
 pytest = "^7.3.1"
 mypy = "^1.2.0"
 types-toml = "^0.10.8.6"
 types-pyyaml = "^6.0.12.9"
-coverage = "^7.2.5"
+git-changelog = "^1.0.1"
+duty = "^0.11.0"
+pytest-cov = "^4.0.0"
+safety = "^2.3.5"
+griffe = "^0.27.5"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1.9"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 mike = "^1.1.2"
+mkdocs-gen-files = "^0.5.0"
+
+[tool.isort]
+profile = "black"
+
+[tool.pylint.format]
+max-line-length = "88"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `typer_config-0.1.3/typer_config/__typing.py` & `typer_config-0.2.0/typer_config/__typing.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.3/typer_config/loaders.py` & `typer_config-0.2.0/typer_config/loaders.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 These loaders must implement the `typer_config.__typing.ConfigLoader` interface.
 """
 import json
 import sys
 
 from .__typing import (
     ConfigDict,
-    ConfigLoader,
     ConfigDictAccessorPath,
+    ConfigLoader,
     NoArgCallable,
     TyperParameterValue,
 )
 
 USING_TOMLLIB = False
 TOML_MISSING = True
 YAML_MISSING = True
+DOTENV_MISSING = True
 
 
 if sys.version_info >= (3, 11):  # pragma: no cover
     import tomllib  # type: ignore
 
     TOML_MISSING = False
     USING_TOMLLIB = True
@@ -38,14 +39,21 @@
 try:  # pragma: no cover
     import yaml
 
     YAML_MISSING = False
 except ImportError:  # pragma: no cover
     pass
 
+try:  # pragma: no cover
+    import dotenv
+
+    DOTENV_MISSING = False
+except ImportError:  # pragma: no cover
+    pass
+
 
 def subpath_loader(
     loader: ConfigLoader, dictpath: ConfigDictAccessorPath
 ) -> ConfigLoader:
     """Modify a loader to return a subpath of the dictionary from file.
 
     Parameters
@@ -169,7 +177,32 @@
         with open(param_value, "rb") as _file:
             conf = tomllib.load(_file)  # type: ignore
     else:  # pragma: no cover
         with open(param_value, "r", encoding="utf-8") as _file:
             conf = toml.load(_file)  # type: ignore
 
     return conf
+
+
+def dotenv_loader(param_value: TyperParameterValue) -> ConfigDict:
+    """Dotenv file loader
+
+    Parameters
+    ----------
+    param_value : TyperParameterValue
+        path of YAML file
+
+    Returns
+    -------
+    ConfigDict
+        dictionary loaded from file
+    """
+
+    if DOTENV_MISSING:  # pragma: no cover
+        raise ModuleNotFoundError("Please install the python-dotenv library.")
+
+    with open(param_value, "r", encoding="utf-8") as _file:
+        # NOTE: I'm using a stream here so that the loader
+        # will raise an exception when the file doesn't exist.
+        conf: ConfigDict = dotenv.dotenv_values(stream=_file)
+
+    return conf
```

### Comparing `typer_config-0.1.3/PKG-INFO` & `typer_config-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: typer-config
-Version: 0.1.3
+Version: 0.2.0
 Summary: Utilities for working with configuration files in typer CLIs. 
 Home-page: https://maxb2.github.io/typer-config/
 License: MIT
-Keywords: typer,config,configuration,configuration-file,yaml,toml,json,cli
+Keywords: typer,config,configuration,configuration-file,yaml,toml,json,dotenv,cli
 Author: Matt Anderson
 Author-email: matt@manderscience.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
@@ -27,25 +27,33 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: all
+Provides-Extra: python-dotenv
 Provides-Extra: toml
 Provides-Extra: yaml
+Requires-Dist: python-dotenv ; extra == "python-dotenv" or extra == "all"
 Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml" or extra == "all"
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "toml" or extra == "all"
 Requires-Dist: typer (>=0,<1)
 Project-URL: Documentation, https://maxb2.github.io/typer-config/
 Project-URL: Repository, https://github.com/maxb2/typer-config
 Description-Content-Type: text/markdown
 
 # typer-config
 
+[![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/maxb2/typer-config/ci.yml?branch=main&style=flat-square)](https://github.com/maxb2/typer-config/actions/workflows/ci.yml)
+[![Codecov](https://img.shields.io/codecov/c/github/maxb2/typer-config?style=flat-square)](https://app.codecov.io/gh/maxb2/typer-config)
+[![PyPI](https://img.shields.io/pypi/v/typer-config?style=flat-square)](https://pypi.org/project/typer-config/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/typer-config?style=flat-square)](https://pypi.org/project/typer-config/#history)
+[![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/typer-config?style=flat-square)](https://libraries.io/pypi/typer-config)
+
 This is a collection of utilities to use configuration files to set parameters for a [typer](https://github.com/tiangolo/typer) CLI.
 It is useful for typer commands with many options/arguments so you don't have to constantly rewrite long commands.
 This package was inspired by [phha/click_config_file](https://github.com/phha/click_config_file) and prototyped in [this issue](https://github.com/tiangolo/typer/issues/86#issuecomment-996374166). It allows you to set values for CLI parameters using a configuration file. 
 
 ## Installation
 
 ```bash
@@ -61,8 +69,8 @@
 # Long commands like this:
 $ my-typer-app --opt1 foo --opt2 bar arg1 arg2
 
 # Can become this:
 $ my-typer-app --config config.yml
 ```
 
-See the [documentation](https://maxb2.github.io/typer-config/examples/) for more examples using typer-config.
+See the [documentation](https://maxb2.github.io/typer-config/latest/examples/simple_yaml/) for more examples using typer-config.
```

