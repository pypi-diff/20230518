# Comparing `tmp/pplkit-0.0.0.tar.gz` & `tmp/pplkit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pplkit-0.0.0.tar", last modified: Fri Apr  1 03:36:31 2022, max compression
+gzip compressed data, was "pplkit-0.1.0.tar", last modified: Thu May 18 21:46:48 2023, max compression
```

## Comparing `pplkit-0.0.0.tar` & `pplkit-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 03:36:31.393939 pplkit-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-04-01 03:36:02.000000 pplkit-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-04-01 03:36:31.393939 pplkit-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-04-01 03:36:02.000000 pplkit-0.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-01 03:36:31.393939 pplkit-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-04-01 03:36:02.000000 pplkit-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 03:36:31.393939 pplkit-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 03:36:31.393939 pplkit-0.0.0/src/pplkit/
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-04-01 03:36:02.000000 pplkit-0.0.0/src/pplkit/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 03:36:02.000000 pplkit-0.0.0/src/pplkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 03:36:31.393939 pplkit-0.0.0/src/pplkit/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 03:36:02.000000 pplkit-0.0.0/src/pplkit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-04-01 03:36:02.000000 pplkit-0.0.0/src/pplkit/data/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     4814 2022-04-01 03:36:02.000000 pplkit-0.0.0/src/pplkit/data/io.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 03:36:31.393939 pplkit-0.0.0/src/pplkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-04-01 03:36:30.000000 pplkit-0.0.0/src/pplkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-04-01 03:36:31.000000 pplkit-0.0.0/src/pplkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 03:36:30.000000 pplkit-0.0.0/src/pplkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 03:36:20.000000 pplkit-0.0.0/src/pplkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-04-01 03:36:31.000000 pplkit-0.0.0/src/pplkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-01 03:36:31.000000 pplkit-0.0.0/src/pplkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:46:48.349671 pplkit-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-18 21:46:10.000000 pplkit-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-18 21:46:48.349671 pplkit-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-18 21:46:10.000000 pplkit-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 21:46:10.000000 pplkit-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 21:46:48.349671 pplkit-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:46:48.345671 pplkit-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:46:48.345671 pplkit-0.1.0/src/pplkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:46:10.000000 pplkit-0.1.0/src/pplkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:46:48.349671 pplkit-0.1.0/src/pplkit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:46:10.000000 pplkit-0.1.0/src/pplkit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-18 21:46:10.000000 pplkit-0.1.0/src/pplkit/data/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-18 21:46:10.000000 pplkit-0.1.0/src/pplkit/data/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:46:48.345671 pplkit-0.1.0/src/pplkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-18 21:46:48.000000 pplkit-0.1.0/src/pplkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-18 21:46:48.000000 pplkit-0.1.0/src/pplkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:46:48.000000 pplkit-0.1.0/src/pplkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 21:46:48.000000 pplkit-0.1.0/src/pplkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 21:46:48.000000 pplkit-0.1.0/src/pplkit.egg-info/top_level.txt
```

### Comparing `pplkit-0.0.0/LICENSE` & `pplkit-0.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2022, IHME Math Sciences
+Copyright (c) 2023, IHME Math Sciences
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `pplkit-0.0.0/src/pplkit/data/interface.py` & `pplkit-0.1.0/src/pplkit/data/interface.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import partial
 from pathlib import Path
-from typing import Any, Dict, Tuple
+from typing import Any
 
-from pplkit.data.io import DataIO, data_io_dict
+from pplkit.data.io import DataIO, dataio_dict
 
 
 class DataInterface:
     """Data interface that store important directories and automatically read
     and write data to the stored directories based on their data types.
 
     Parameters
@@ -14,46 +14,88 @@
     dirs
         Directories to manage with directory's name as the name of the keyword
         argument's name and directory's path as the value of the keyword
         argument's value.
 
     """
 
-    data_io_dict: Dict[str, DataIO] = data_io_dict
+    dataio_dict: dict[str, DataIO] = dataio_dict
     """A dictionary that maps the file extensions to the corresponding data io
     class. This is a module-level variable from
-    :py:data:`pplkit.data.io.data_io_dict`.
+    :py:data:`pplkit.data.io.dataio_dict`.
 
     :meta hide-value:
 
     """
 
-    def __init__(self, **dirs: Dict[str, str | Path]):
+    def __init__(self, **dirs: dict[str, str | Path]) -> None:
+        self.keys = []
         for key, value in dirs.items():
-            setattr(self, key, Path(value))
-            setattr(self, f"load_{key}", partial(self.load, key=key))
-            setattr(self, f"dump_{key}", partial(self.dump, key=key))
-        self.keys = list(dirs.keys())
+            self.add_dir(key, value)
 
-    def get_fpath(self, *fparts: Tuple[str, ...], key: str = "") -> Path:
+    def add_dir(self, key: str, value: str | Path, exist_ok: bool = False) -> None:
+        """Add a directory to instance. If the directory already exist
+
+        Parameters
+        ----------
+        key
+            Directory name.
+        value
+            Directory path.
+        exist_ok
+            If ``exist_ok=True`` and ``key`` already exists in the current
+            instance it will raise an error. Otherwise it will overwrite the
+            path corresponding to the ``key``.
+
+        Raises
+        ------
+        ValueError
+            Raised when ``exist_ok=False`` and ``key`` already exists.
+
+        """
+        if (not exist_ok) and (key in self.keys):
+            raise ValueError(f"{key} already exists")
+        setattr(self, key, Path(value))
+        setattr(self, f"load_{key}", partial(self.load, key=key))
+        setattr(self, f"dump_{key}", partial(self.dump, key=key))
+        if key not in self.keys:
+            self.keys.append(key)
+
+    def remove_dir(self, key: str) -> None:
+        """Remove a directory from the current set of directories.
+
+        Parameters
+        ----------
+        key
+            Directory name
+
+        """
+        if key in self.keys:
+            delattr(self, key)
+            delattr(self, f"load_{key}")
+            delattr(self, f"dump_{key}")
+            self.keys.remove(key)
+
+    def get_fpath(self, *fparts: tuple[str, ...], key: str = "") -> Path:
         """Get the file path from the name of the directory and the sub-parts
         under the directory.
 
         Parameters
         ----------
         fparts
             Subdirectories or the file name.
         key
             The name of the directory stored in the class.
 
         """
         return getattr(self, key, Path(".")) / "/".join(map(str, fparts))
 
-    def load(self, *fparts: Tuple[str, ...], key: str = "",
-             **options: Dict[str, Any]) -> Any:
+    def load(
+        self, *fparts: tuple[str, ...], key: str = "", **options: dict[str, Any]
+    ) -> Any:
         """Load data from given directory.
 
         Parameters
         ----------
         fparts
             Subdirectories or the file name.
         key
@@ -64,18 +106,24 @@
         Returns
         -------
         Any
             Data loaded from the given path.
 
         """
         fpath = self.get_fpath(*fparts, key=key)
-        return self.data_io_dict[fpath.suffix].load(fpath, **options)
+        return self.dataio_dict[fpath.suffix].load(fpath, **options)
 
-    def dump(self, obj: Any, *fparts: str, key: str = "",
-             mkdir: bool = True, **options: Dict[str, Any]):
+    def dump(
+        self,
+        obj: Any,
+        *fparts: str,
+        key: str = "",
+        mkdir: bool = True,
+        **options: dict[str, Any],
+    ):
         """Dump data to the given directory.
 
         Parameters
         ----------
         obj
             Provided data object.
         fparts
@@ -86,15 +134,15 @@
             If true, it will automatically create the parent directory. The
             default is true.
         options
             Extra arguments for the dump function.
 
         """
         fpath = self.get_fpath(*fparts, key=key)
-        self.data_io_dict[fpath.suffix].dump(obj, fpath, mkdir=mkdir, **options)
+        self.dataio_dict[fpath.suffix].dump(obj, fpath, mkdir=mkdir, **options)
 
     def __repr__(self) -> str:
         expr = f"{type(self).__name__}(\n"
         for key in self.keys:
             expr += f"    {key}={getattr(self, key)},\n"
         expr += ")"
         return expr
```

### Comparing `pplkit-0.0.0/src/pplkit/data/io.py` & `pplkit-0.1.0/src/pplkit/data/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, Dict, List, Tuple, Type
+from typing import Any, Type
 
 import dill
 import pandas as pd
+import tomli
+import tomli_w
 import yaml
 
 
 class DataIO(ABC):
-    """Bridge class that unifies the file I/O for different data types.
+    """Bridge class that unifies the file I/O for different data types."""
 
-    """
-
-    fextns: Tuple[str] = ("",)
+    fextns: tuple[str, ...] = ("",)
     """The file extensions. When loading a file, it will be used to check if
     the file extension matches.
 
     """
-    dtypes: Tuple[Type] = (object,)
+    dtypes: tuple[Type, ...] = (object,)
     """The data types. When dumping the data, it will be used to check if the
     data type matches.
 
     """
 
     @abstractmethod
     def _load(self, fpath: Path, **options) -> Any:
@@ -83,104 +83,112 @@
         if not isinstance(obj, self.dtypes):
             raise TypeError(f"Data must be an instance of {self.dtypes}.")
         if mkdir:
             fpath.parent.mkdir(parents=True, exist_ok=True)
         self._dump(obj, fpath, **options)
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}(fextns={self.fextns})"
+        return f"{type(self).__name__}()"
 
 
 class CSVIO(DataIO):
-
-    fextns: Tuple[str] = (".csv",)
-    dtypes: Tuple[Type] = (pd.DataFrame,)
+    fextns: tuple[str, ...] = (".csv",)
+    dtypes: tuple[Type, ...] = (pd.DataFrame,)
 
     def _load(self, fpath: Path, **options) -> pd.DataFrame:
         return pd.read_csv(fpath, **options)
 
     def _dump(self, obj: pd.DataFrame, fpath: Path, **options):
         options = dict(index=False) | options
         obj.to_csv(fpath, **options)
 
 
 class PickleIO(DataIO):
-
-    fextns: Tuple[str] = (".pkl", ".pickle")
+    fextns: tuple[str, ...] = (".pkl", ".pickle")
 
     def _load(self, fpath: Path, **options) -> Any:
         with open(fpath, "rb") as f:
             return dill.load(f, **options)
 
     def _dump(self, obj: Any, fpath: Path, **options):
         with open(fpath, "wb") as f:
             return dill.dump(obj, f, **options)
 
 
 class YAMLIO(DataIO):
+    fextns: tuple[str, ...] = (".yml", ".yaml")
+    dtypes: tuple[Type, ...] = (dict, list)
 
-    fextns: Tuple[str] = (".yml", ".yaml")
-    dtypes: Tuple[Type] = (dict, list)
-
-    def _load(self, fpath: Path, **options) -> Dict | List:
+    def _load(self, fpath: Path, **options) -> dict | list:
         options = dict(Loader=yaml.SafeLoader) | options
         with open(fpath, "r") as f:
             return yaml.load(f, **options)
 
-    def _dump(self, obj: Dict | List, fpath: Path, **options):
+    def _dump(self, obj: dict | list, fpath: Path, **options):
         options = dict(Dumper=yaml.SafeDumper) | options
         with open(fpath, "w") as f:
             return yaml.dump(obj, f, **options)
 
 
 class ParquetIO(DataIO):
-
-    fextns: Tuple[str] = (".parquet",)
-    dtypes: Tuple[Type] = (pd.DataFrame,)
+    fextns: tuple[str, ...] = (".parquet",)
+    dtypes: tuple[Type, ...] = (pd.DataFrame,)
 
     def _load(self, fpath: Path, **options) -> pd.DataFrame:
         options = dict(engine="pyarrow") | options
         return pd.read_parquet(fpath, **options)
 
     def _dump(self, obj: pd.DataFrame, fpath: Path, **options):
         options = dict(engine="pyarrow") | options
         obj.to_parquet(fpath, **options)
 
 
 class JSONIO(DataIO):
+    fextns: tuple[str, ...] = (".json",)
+    dtypes: tuple[Type, ...] = (dict, list)
 
-    fextns: Tuple[str] = (".json",)
-    dtypes: Tuple[Type] = (dict, list)
-
-    def _load(self, fpath: Path, **options) -> Dict | List:
+    def _load(self, fpath: Path, **options) -> dict | list:
         with open(fpath, "r") as f:
             return json.load(f, **options)
 
-    def _dump(self, obj: Dict | List, fpath: Path, **options):
+    def _dump(self, obj: dict | list, fpath: Path, **options):
         with open(fpath, "w") as f:
             json.dump(obj, f, **options)
 
 
-data_io_instances: List[DataIO] = [
-    CSVIO(),
-    YAMLIO(),
-    PickleIO(),
-    ParquetIO(),
-    JSONIO(),
-]
-"""Instances of all the data ios. These are singletons and module variables.
+class TOMLIO(DataIO):
+    fextns: tuple[str, ...] = (".toml",)
+    dtypes: tuple[Type, ...] = (dict,)
 
-:meta hide-value:
+    def _load(self, fpath: Path, **options) -> dict:
+        with open(fpath, "rb") as f:
+            return tomli.load(f, **options)
 
-"""
+    def _dump(self, obj: dict, fpath: Path, **options):
+        with open(fpath, "wb") as f:
+            tomli_w.dump(obj, f)
 
 
-data_io_dict: Dict[str, DataIO] = {
-    fextn: data_io
-    for data_io in data_io_instances for fextn in data_io.fextns
+csvio = CSVIO()
+yamlio = YAMLIO()
+pickleio = PickleIO()
+parquetio = ParquetIO()
+jsonio = JSONIO()
+tomlio = TOMLIO()
+
+_dataio_list: list[DataIO] = [
+    csvio,
+    yamlio,
+    pickleio,
+    parquetio,
+    jsonio,
+    tomlio,
+]
+
+
+dataio_dict: dict[str, DataIO] = {
+    fextn: dataio for dataio in _dataio_list for fextn in dataio.fextns
 }
 """Instances of data ios, organized in a dictionary with key as the file
-extensions for each :py:class:`DataIO` class.
-
-:meta hide-value:
+extensions for each :class:`DataIO` class.
 
 """
```

