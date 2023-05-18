# Comparing `tmp/typer_config-0.2.0.tar.gz` & `tmp/typer_config-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_config-0.2.0.tar", max compression
+gzip compressed data, was "typer_config-0.3.0.tar", max compression
```

## Comparing `typer_config-0.2.0.tar` & `typer_config-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-16 04:06:27.574721 typer_config-0.2.0/LICENSE
--rw-r--r--   0        0        0     1838 2023-05-16 04:34:58.786785 typer_config-0.2.0/README.md
--rw-r--r--   0        0        0     2454 2023-05-18 00:01:41.974428 typer_config-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3945 2023-05-17 23:52:39.623396 typer_config-0.2.0/typer_config/__init__.py
--rw-r--r--   0        0        0     1089 2023-05-16 04:06:27.578055 typer_config-0.2.0/typer_config/__typing.py
--rw-r--r--   0        0        0     4560 2023-05-17 23:52:39.623396 typer_config-0.2.0/typer_config/loaders.py
--rw-r--r--   0        0        0     3841 1970-01-01 00:00:00.000000 typer_config-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-16 04:06:27.574721 typer_config-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1840 2023-05-18 01:01:35.696589 typer_config-0.3.0/README.md
+-rw-r--r--   0        0        0     2454 2023-05-18 02:46:44.745316 typer_config-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3706 2023-05-18 02:25:55.528865 typer_config-0.3.0/typer_config/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-16 04:06:27.578055 typer_config-0.3.0/typer_config/__typing.py
+-rw-r--r--   0        0        0     5957 2023-05-18 02:33:38.242837 typer_config-0.3.0/typer_config/loaders.py
+-rw-r--r--   0        0        0     3843 1970-01-01 00:00:00.000000 typer_config-0.3.0/PKG-INFO
```

### Comparing `typer_config-0.2.0/LICENSE` & `typer_config-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_config-0.2.0/README.md` & `typer_config-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 ## Installation
 
 ```bash
 $ pip install typer-config[all]
 ```
 
-> **Note**: that will include libraries for reading from YAML and TOML files as well.
-  Feel free to leave off the optional dependencies if you don't need YAML or TOML capabilities.
+> **Note**: that will include libraries for reading from YAML, TOML, and Dotenv files as well.
+  Feel free to leave off the optional dependencies if you don't need those capabilities.
 
 ## Usage
 
 ```bash
 # Long commands like this:
 $ my-typer-app --opt1 foo --opt2 bar arg1 arg2
```

### Comparing `typer_config-0.2.0/pyproject.toml` & `typer_config-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-config"
-version = "0.2.0"
+version = "0.3.0"
 description = "Utilities for working with configuration files in typer CLIs. "
 authors = ["Matt Anderson <matt@manderscience.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "typer_config"}]
 repository = "https://github.com/maxb2/typer-config"
 documentation = "https://maxb2.github.io/typer-config/"
```

### Comparing `typer_config-0.2.0/typer_config/__init__.py` & `typer_config-0.3.0/typer_config/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,146 +7,108 @@
 from .__typing import ConfigLoader, ConfigParameterCallback, TyperParameterValue
 from .loaders import dotenv_loader, json_loader, toml_loader, yaml_loader
 
 
 def conf_callback_factory(loader: ConfigLoader) -> ConfigParameterCallback:
     """Typer configuration callback factory.
 
-    Parameters
-    ----------
-    loader : ConfigLoader
-        Config loader function that takes the value passed to the typer CLI and
-        returns a dictionary that is applied to the click context's default map.
-
-    Returns
-    -------
-    ConfigParameterCallback
-        Configuration parameter callback function.
+    Args:
+        loader (ConfigLoader): Config loader function that takes the value
+            passed to the typer CLI and returns a dictionary that is
+            applied to the click context's default map.
+
+    Returns:
+        ConfigParameterCallback: Configuration parameter callback function.
     """
 
     def _callback(
         ctx: Context, param: CallbackParam, param_value: TyperParameterValue
     ) -> TyperParameterValue:
         """Generated typer config parameter callback.
 
-        Parameters
-        ----------
-        ctx : typer.Context
-            typer context (automatically passed)
-        param : typer.CallbackParam
-            typer callback parameter (automatically passed)
-        param_value : TyperParameterValue
-            parameter value passed to typer (automatically passed)
-
-        Returns
-        -------
-        TyperParameterValue
-            must return back the given parameter
-
-        Raises
-        ------
-        typer.BadParameter
-            bad parameter value
+        Args:
+            ctx (typer.Context): typer context (automatically passed)
+            param (typer.CallbackParam): typer callback parameter (automatically passed)
+            param_value (TyperParameterValue): parameter value passed to typer
+                (automatically passed)
+
+        Raises:
+            BadParameter: bad parameter value
+
+        Returns:
+            TyperParameterValue: must return back the given parameter
         """
         try:
             conf = loader(param_value)  # Load config file
             ctx.default_map = ctx.default_map or {}  # Initialize the default map
             ctx.default_map.update(conf)  # Merge the config Dict into default_map
         except Exception as ex:
             raise BadParameter(str(ex), ctx=ctx, param=param) from ex
         return param_value
 
     return _callback
 
 
 yaml_conf_callback: ConfigParameterCallback = conf_callback_factory(yaml_loader)
-"""YAML configuration callback for a typer parameter.
+"""YAML typer config parameter callback.
 
-Parameters
-----------
-ctx : typer.Context
-    typer context (automatically passed)
-param : typer.CallbackParam
-    typer callback parameter (automatically passed)
-param_value : TyperParameterValue
-    parameter value passed to typer (automatically passed)
-
-Returns
--------
-TyperParameterValue
-    must return back the given parameter
-
-Raises
-------
-typer.BadParameter
-    bad parameter value
+Args:
+    ctx (typer.Context): typer context (automatically passed)
+    param (typer.CallbackParam): typer callback parameter (automatically passed)
+    param_value (TyperParameterValue): parameter value passed to typer (automatically
+        passed)
+
+Raises:
+    BadParameter: bad parameter value
+
+Returns:
+    TyperParameterValue: must return back the given parameter
 """
 
 json_conf_callback: ConfigParameterCallback = conf_callback_factory(json_loader)
-"""JSON configuration callback for a typer parameter.
+"""JSON typer config parameter callback.
+
+Args:
+    ctx (typer.Context): typer context (automatically passed)
+    param (typer.CallbackParam): typer callback parameter (automatically passed)
+    param_value (TyperParameterValue): parameter value passed to typer (automatically
+        passed)
 
-Parameters
-----------
-ctx : typer.Context
-    typer context (automatically passed)
-param : typer.CallbackParam
-    typer callback parameter (automatically passed)
-param_value : TyperParameterValue
-    parameter value passed to typer (automatically passed)
-
-Returns
--------
-TyperParameterValue
-    must return back the given parameter
-
-Raises
-------
-typer.BadParameter
-    bad parameter value
+Raises:
+    BadParameter: bad parameter value
+
+Returns:
+    TyperParameterValue: must return back the given parameter
 """
 
 
 toml_conf_callback: ConfigParameterCallback = conf_callback_factory(toml_loader)
-"""TOML configuration callback for a typer parameter.
+"""TOML typer config parameter callback.
+
+Args:
+    ctx (typer.Context): typer context (automatically passed)
+    param (typer.CallbackParam): typer callback parameter (automatically passed)
+    param_value (TyperParameterValue): parameter value passed to typer (automatically
+        passed)
+
+Raises:
+    BadParameter: bad parameter value
 
-Parameters
-----------
-ctx : typer.Context
-    typer context (automatically passed)
-param : typer.CallbackParam
-    typer callback parameter (automatically passed)
-param_value : TyperParameterValue
-    parameter value passed to typer (automatically passed)
-
-Returns
--------
-TyperParameterValue
-    must return back the given parameter
-
-Raises
-------
-typer.BadParameter
-    bad parameter value
+Returns:
+    TyperParameterValue: must return back the given parameter
 """
 
 dotenv_conf_callback: ConfigParameterCallback = conf_callback_factory(dotenv_loader)
-"""Dotenv configuration callback for a typer parameter.
+"""Dotenv typer config parameter callback.
+
+Args:
+    ctx (typer.Context): typer context (automatically passed)
+    param (typer.CallbackParam): typer callback parameter (automatically passed)
+    param_value (TyperParameterValue): parameter value passed to typer (automatically
+        passed)
+
+Raises:
+    BadParameter: bad parameter value
 
-Parameters
-----------
-ctx : typer.Context
-    typer context (automatically passed)
-param : typer.CallbackParam
-    typer callback parameter (automatically passed)
-param_value : TyperParameterValue
-    parameter value passed to typer (automatically passed)
-
-Returns
--------
-TyperParameterValue
-    must return back the given parameter
-
-Raises
-------
-typer.BadParameter
-    bad parameter value
+Returns:
+    TyperParameterValue: must return back the given parameter
 """
```

### Comparing `typer_config-0.2.0/typer_config/__typing.py` & `typer_config-0.3.0/typer_config/__typing.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.2.0/typer_config/loaders.py` & `typer_config-0.3.0/typer_config/loaders.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Configuration File Loaders.
 
 These loaders must implement the `typer_config.__typing.ConfigLoader` interface.
 """
 import json
 import sys
+from configparser import ConfigParser
 
 from .__typing import (
     ConfigDict,
     ConfigDictAccessorPath,
     ConfigLoader,
     NoArgCallable,
     TyperParameterValue,
@@ -52,25 +53,35 @@
 
 
 def subpath_loader(
     loader: ConfigLoader, dictpath: ConfigDictAccessorPath
 ) -> ConfigLoader:
     """Modify a loader to return a subpath of the dictionary from file.
 
-    Parameters
-    ----------
-    loader : ConfigLoader
-        loader to modify
-    dictpath : ConfigDictAccessorPath
-        path to the section of the dictionary to return
-
-    Returns
-    -------
-    ConfigLoader
-        sub dictionary loader
+    Examples:
+        The following example reads the values from the `my_app` section in
+        a YAML file structured like this:
+        ```yaml
+        tools:
+            my_app:
+                ... # use these values
+            others: # ignore
+        stuf: # ignore
+        ```
+
+        ```py
+        my_loader = subpath_loader(yaml_loader, ["tools", "my_app"])
+        ```
+
+    Args:
+        loader (ConfigLoader): loader to modify
+        dictpath (ConfigDictAccessorPath): path to the section of dictionary
+
+    Returns:
+        ConfigLoader: sub dictionary loader
     """
 
     def _loader(param_value: str) -> ConfigDict:
         # get original ConfigDict
         conf: ConfigDict = loader(param_value)
 
         # get subpath of dictionary
@@ -80,27 +91,30 @@
 
     return _loader
 
 
 def default_value_loader(
     loader: ConfigLoader, value_getter: NoArgCallable
 ) -> ConfigLoader:
-    """Modify a loader to use a default value if the passed value is false-ish
+    """Modify a loader to use a default value if the passed value is false-ish.
+
+    Examples:
+        The following example lets a user specify a config file, but will load
+        the `pyproject.toml` if they don't.
+
+        ```py
+        pyproject_loader = default_value_loader(toml_loader, lambda: "pyproject.toml")
+        ```
+
+    Args:
+        loader (ConfigLoader): loader to modify
+        value_getter (NoArgCallable): function that returns default value
 
-    Parameters
-    ----------
-    loader : ConfigLoader
-        loader to modify
-    value_getter : NoArgCallable
-        function that returns default value
-
-    Returns
-    -------
-    ConfigLoader
-        modified loader
+    Returns:
+        ConfigLoader: modified loader
     """
 
     def _loader(param_value: str) -> ConfigDict:
         # parameter value was not specified by user
         if not param_value:
             param_value = value_getter()
 
@@ -108,68 +122,62 @@
 
         return conf
 
     return _loader
 
 
 def yaml_loader(param_value: TyperParameterValue) -> ConfigDict:
-    """YAML file loader
+    """YAML file loader.
+
+    Args:
+        param_value (TyperParameterValue): path of YAML file
 
-    Parameters
-    ----------
-    param_value : TyperParameterValue
-        path of YAML file
-
-    Returns
-    -------
-    ConfigDict
-        dictionary loaded from file
+    Raises:
+        ModuleNotFoundError: pyyaml library is not installed
+
+    Returns:
+        ConfigDict: dictionary loaded from file
     """
 
     if YAML_MISSING:  # pragma: no cover
         raise ModuleNotFoundError("Please install the pyyaml library.")
 
     with open(param_value, "r", encoding="utf-8") as _file:
         conf: ConfigDict = yaml.safe_load(_file)
 
     return conf
 
 
 def json_loader(param_value: TyperParameterValue) -> ConfigDict:
-    """JSON file loader
+    """JSON file loader.
+
+    Args:
+        param_value (TyperParameterValue): path of JSON file
 
-    Parameters
-    ----------
-    param_value : TyperParameterValue
-        path of JSON file
-
-    Returns
-    -------
-    ConfigDict
-        dictionary loaded from file
+    Returns:
+        ConfigDict: dictionary loaded from file
     """
 
     with open(param_value, "r", encoding="utf-8") as _file:
         conf: ConfigDict = json.load(_file)
 
     return conf
 
 
 def toml_loader(param_value: TyperParameterValue) -> ConfigDict:
-    """TOML file loader
+    """TOML file loader.
 
-    Parameters
-    ----------
-    param_value : TyperParameterValue
-        path of TOML file
-
-    Returns
-    -------
-    ConfigDict
-        dictionary loaded from file
+    Args:
+        param_value (TyperParameterValue): path of TOML file
+
+    Raises:
+        ModuleNotFoundError: toml library is not installed
+
+    Returns:
+        ConfigDict: dictionary loaded from file
     """
 
     if TOML_MISSING:  # pragma: no cover
         raise ModuleNotFoundError("Please install the toml library.")
 
     conf: ConfigDict = {}
 
@@ -180,29 +188,57 @@
         with open(param_value, "r", encoding="utf-8") as _file:
             conf = toml.load(_file)  # type: ignore
 
     return conf
 
 
 def dotenv_loader(param_value: TyperParameterValue) -> ConfigDict:
-    """Dotenv file loader
+    """Dotenv file loader.
+
+    Args:
+        param_value (TyperParameterValue): path of Dotenv file
 
-    Parameters
-    ----------
-    param_value : TyperParameterValue
-        path of YAML file
-
-    Returns
-    -------
-    ConfigDict
-        dictionary loaded from file
+    Raises:
+        ModuleNotFoundError: python-dotenv library is not installed
+
+    Returns:
+        ConfigDict: dictionary loaded from file
     """
 
     if DOTENV_MISSING:  # pragma: no cover
         raise ModuleNotFoundError("Please install the python-dotenv library.")
 
     with open(param_value, "r", encoding="utf-8") as _file:
         # NOTE: I'm using a stream here so that the loader
         # will raise an exception when the file doesn't exist.
         conf: ConfigDict = dotenv.dotenv_values(stream=_file)
 
     return conf
+
+
+def ini_loader(param_value: TyperParameterValue) -> ConfigDict:
+    """INI file loader
+
+    Note:
+        INI files must have sections at the top level.
+        You probably want to combine this with `subpath_loader`.
+        For example:
+        ```py
+        ini_section_loader = subpath_loader(ini_loader, ["section"])
+        ```
+
+    Args:
+        param_value (TyperParameterValue): path of INI file
+
+    Returns:
+        ConfigDict: dictionary loaded from file
+    """
+
+    ini_parser = ConfigParser()
+    with open(param_value, "r", encoding="utf-8") as _file:
+        ini_parser.read_file(_file)
+
+    conf: ConfigDict = {
+        sect: dict(ini_parser.items(sect)) for sect in ini_parser.sections()
+    }
+
+    return conf
```

### Comparing `typer_config-0.2.0/PKG-INFO` & `typer_config-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-config
-Version: 0.2.0
+Version: 0.3.0
 Summary: Utilities for working with configuration files in typer CLIs. 
 Home-page: https://maxb2.github.io/typer-config/
 License: MIT
 Keywords: typer,config,configuration,configuration-file,yaml,toml,json,dotenv,cli
 Author: Matt Anderson
 Author-email: matt@manderscience.com
 Requires-Python: >=3.8,<4.0
@@ -56,16 +56,16 @@
 
 ## Installation
 
 ```bash
 $ pip install typer-config[all]
 ```
 
-> **Note**: that will include libraries for reading from YAML and TOML files as well.
-  Feel free to leave off the optional dependencies if you don't need YAML or TOML capabilities.
+> **Note**: that will include libraries for reading from YAML, TOML, and Dotenv files as well.
+  Feel free to leave off the optional dependencies if you don't need those capabilities.
 
 ## Usage
 
 ```bash
 # Long commands like this:
 $ my-typer-app --opt1 foo --opt2 bar arg1 arg2
```

