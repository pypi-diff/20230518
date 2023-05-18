# Comparing `tmp/ndradex-0.2.2.tar.gz` & `tmp/ndradex-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ndradex-0.2.2.tar", last modified: Tue Oct 27 13:59:51 2020, max compression
+gzip compressed data, was "ndradex-0.3.0.tar", max compression
```

## Comparing `ndradex-0.2.2.tar` & `ndradex-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-27 13:59:51.681892 ndradex-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1076 2020-10-27 13:59:03.000000 ndradex-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      143 2020-10-27 13:59:03.000000 ndradex-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     9899 2020-10-27 13:59:51.681892 ndradex-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7739 2020-10-27 13:59:03.000000 ndradex-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-27 13:59:51.681892 ndradex-0.2.2/ndradex/
--rw-r--r--   0 runner    (1001) docker     (116)     1361 2020-10-27 13:59:03.000000 ndradex-0.2.2/ndradex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-27 13:59:51.681892 ndradex-0.2.2/ndradex/bin/
--rw-r--r--   0 runner    (1001) docker     (116)     2484 2020-10-27 13:59:04.000000 ndradex-0.2.2/ndradex/bin/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     6748 2020-10-27 13:59:03.000000 ndradex-0.2.2/ndradex/db.py
--rw-r--r--   0 runner    (1001) docker     (116)    12170 2020-10-27 13:59:03.000000 ndradex-0.2.2/ndradex/grid.py
--rw-r--r--   0 runner    (1001) docker     (116)     3768 2020-10-27 13:59:03.000000 ndradex-0.2.2/ndradex/radex.py
--rw-r--r--   0 runner    (1001) docker     (116)     1907 2020-10-27 13:59:03.000000 ndradex-0.2.2/ndradex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-27 13:59:51.681892 ndradex-0.2.2/ndradex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9899 2020-10-27 13:59:51.000000 ndradex-0.2.2/ndradex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      307 2020-10-27 13:59:51.000000 ndradex-0.2.2/ndradex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-27 13:59:51.000000 ndradex-0.2.2/ndradex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      144 2020-10-27 13:59:51.000000 ndradex-0.2.2/ndradex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-10-27 13:59:51.000000 ndradex-0.2.2/ndradex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      829 2020-10-27 13:59:51.681892 ndradex-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      597 2020-10-27 13:59:03.000000 ndradex-0.2.2/setup.py
+-rw-r--r--   0        0        0     1076 2023-05-18 17:37:48.900780 ndradex-0.3.0/LICENSE
+-rw-r--r--   0        0        0      416 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/__init__.py
+-rw-r--r--   0        0        0      150 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0      377 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       39 2023-05-18 17:37:49.548783 ndradex-0.3.0/ndradex/bin/.git
+-rw-r--r--   0        0        0      958 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/.github/workflows/formula.yml
+-rw-r--r--   0        0        0      412 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/.github/workflows/tests.yml
+-rw-r--r--   0        0        0        7 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/.gitignore
+-rw-r--r--   0        0        0      440 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/CITATION.cff
+-rw-r--r--   0        0        0      902 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/Formula/radex.rb
+-rw-r--r--   0        0        0     1076 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/LICENSE
+-rw-r--r--   0        0        0     1304 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/Makefile
+-rw-r--r--   0        0        0     2202 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/README.md
+-rw-r--r--   0        0        0     3569 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/consts.py
+-rw-r--r--   0        0        0     6742 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/db.py
+-rw-r--r--   0        0        0    12538 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/grid.py
+-rw-r--r--   0        0        0      462 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/io.py
+-rw-r--r--   0        0        0     3440 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/radex.py
+-rw-r--r--   0        0        0      874 2023-05-18 17:37:48.900780 ndradex-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 ndradex-0.3.0/PKG-INFO
```

### Comparing `ndradex-0.2.2/LICENSE` & `ndradex-0.3.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2020 Akio Taniguchi
+Copyright (c) 2019-2023 Akio Taniguchi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ndradex-0.2.2/ndradex/db.py` & `ndradex-0.3.0/ndradex/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 __all__ = ["LAMDA"]
 
 
-# from standard library
+# tandard library
 import re
 import warnings
-from functools import wraps
+from functools import partial, wraps
 from logging import getLogger
 from pathlib import Path
 from urllib.parse import urlparse
 
 
-# from dependent packages
-import ndradex
+# dependencies
 import numpy as np
+from .consts import LAMDA_ALIASES
 
 
 logger = getLogger(__name__)
 
 
 def cache(func):
     """Decorator for caching result of a method."""
@@ -32,16 +32,15 @@
         return result
 
     return wrapped
 
 
 class LAMDA:
     def __init__(self, query, dir="."):
-        if query in ndradex.config["lamda"]:
-            query = ndradex.config["lamda"][query]
+        query = LAMDA_ALIASES.get(query, query)
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
 
             tables = get_tables(query)
             path = get_data_path(query, dir)
 
@@ -90,28 +89,28 @@
     @property
     @cache
     def n_crit(self):
         """Critical densities in units of cm^-3."""
         # lazy import of astropy-related things
         from astroquery.lamda.utils import ncrit
 
-        tables = (self._collrates, self._transitions, self._levels)
+        @np.vectorize
+        def func(T_kin, index_u, index_l):
+            tables = (self._collrates, self._transitions, self._levels)
+            return ncrit(tables, index_u, index_l, T_kin).value
+
+        funcs = {}
 
-        funcs = []
         for qn_ul in self.qn_ul:
             index_u = self._transitions.loc[qn_ul]["Upper"]
             index_l = self._transitions.loc[qn_ul]["Lower"]
 
-            @np.vectorize
-            def func(T_kin):
-                return ncrit(tables, index_u, index_l, T_kin).value
-
-            funcs.append(func)
+            funcs[qn_ul] = partial(func, index_u=index_u, index_l=index_l)
 
-        return dict(zip(self.qn_ul, funcs))
+        return funcs
 
     def __enter__(self):
         """Create a temporary LAMDA data inside a context block."""
         # lazy import of astropy-related things
         from astroquery.lamda import write_lamda_datafile
 
         tables = (self._collrates, self._transitions, self._levels)
```

### Comparing `ndradex-0.2.2/ndradex/grid.py` & `ndradex-0.3.0/ndradex/grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,62 @@
 __all__ = ["run"]
 
 
 # standard library
+from concurrent.futures import ProcessPoolExecutor
 from enum import Enum, auto
 from itertools import product, repeat
 from pathlib import Path
+from random import getrandbits
 from tempfile import TemporaryDirectory
 
 
 # dependencies
-import ndradex
 import numpy as np
 import pandas as pd
 import xarray as xr
 from tqdm import tqdm
+from .consts import (
+    DV,
+    GEOM,
+    N_E,
+    N_H,
+    N_H2,
+    N_HE,
+    N_HP,
+    N_MOL,
+    N_OH2,
+    N_PARALLEL,
+    N_PH2,
+    PROGRESS,
+    RADEX_BIN,
+    SQUEEZE,
+    T_BG,
+    T_KIN,
+    TIMEOUT,
+)
+from .db import LAMDA
+from .radex import run as run_radex
 
 
 # constants
 class Dims(Enum):
-    QN_ul = auto()
-    T_kin = auto()
-    N_mol = auto()
+    QN_ul = "QN_ul"
+    T_kin = "T_kin"
+    N_mol = "N_mol"
     n_H2 = "H2"
     n_pH2 = "p-H2"
     n_oH2 = "o-H2"
     n_e = "e"
     n_H = "H"
     n_He = "He"
     n_Hp = "H+"
-    T_bg = auto()
-    dv = auto()
-    geom = auto()
+    T_bg = "T_bg"
+    dv = "dv"
+    geom = "geom"
 
 
 class Vars(Enum):
     E_u = auto()
     freq = auto()
     wavel = auto()
     T_ex = auto()
@@ -43,35 +65,34 @@
     pop_u = auto()
     pop_l = auto()
     I = auto()
     F = auto()
 
 
 # main function
-@ndradex.utils.set_defaults(**ndradex.config["grid"])
 def run(
     query,
     QN_ul,
-    T_kin=100,
-    N_mol=1e15,
-    n_H2=1e3,
-    n_pH2=None,
-    n_oH2=None,
-    n_e=None,
-    n_H=None,
-    n_He=None,
-    n_Hp=None,
-    T_bg=2.73,
-    dv=1.0,
-    geom="uni",
+    T_kin=T_KIN,
+    N_mol=N_MOL,
+    n_H2=N_H2,
+    n_pH2=N_PH2,
+    n_oH2=N_OH2,
+    n_e=N_E,
+    n_H=N_H,
+    n_He=N_HE,
+    n_Hp=N_HP,
+    T_bg=T_BG,
+    dv=DV,
+    geom=GEOM,
     *,
-    squeeze=True,
-    progress=True,
-    timeout=None,
-    n_procs=None,
+    squeeze=SQUEEZE,
+    progress=PROGRESS,
+    timeout=TIMEOUT,
+    n_procs=N_PARALLEL,
     work_dir=None,
 ):
     """Run grid RADEX calculation and get results as xarray.Dataset.
 
     This is the main function of ndRADEX. It provides 13 parameters
     which can be griddable (i.e., both scalar and array are accepted).
     The output is an xarray's Dataset of multi-dimensional DataArrays
@@ -186,15 +207,15 @@
         n_Hp,
         T_bg,
         dv,
         geom,
     )
 
     with TemporaryDirectory(dir=work_dir) as temp_dir:
-        with ndradex.db.LAMDA(query, temp_dir) as lamda:
+        with LAMDA(query, temp_dir) as lamda:
             # make an empty dataset and flattened args
             dataset = get_empty_dataset(lamda, empty)
             iterables = [
                 generate_inputs(lamda, empty),
                 generate_radex_paths(lamda, empty),
                 repeat(timeout),
             ]
@@ -213,20 +234,20 @@
 
 # sub functions
 def generate_inputs(lamda, empty):
     """Generate RADEX input string iteratively."""
     template = get_input_template(lamda, empty)
 
     for kwargs in generate_kwargs(lamda, empty):
-        yield template.format(**kwargs)
+        yield template.format(**kwargs).split("\n")
 
 
 def generate_radex_paths(lamda, empty):
     """Generate RADEX path iteratively."""
-    path = str(ndradex.RADEX_BINPATH / "radex-{geom}")
+    path = str(RADEX_BIN / "radex-{geom}")
 
     for kwargs in generate_kwargs(lamda, empty):
         yield path.format(geom=kwargs[Dims.geom.name])
 
 
 def get_empty_dataset(lamda, empty):
     """Make an empty xarray.Dataset for storing DataArrays."""
@@ -236,19 +257,20 @@
 
 
 def execute(dataset, *iterables, dir=".", progress=True, n_procs=None):
     """Run grid RADEX calculation and store results into a dataset."""
     total = np.prod(list(dataset.dims.values()))
     outfile = Path(dir, "grid.out").expanduser().resolve()
 
-    with outfile.open("w", buffering=1) as f, ndradex.utils.runner(
-        n_procs
-    ) as runner, tqdm(total=total, disable=not progress) as bar:
-        # write outputs to a single file
-        for output in runner.map(ndradex.radex.run, *iterables):
+    # fmt: off
+    with tqdm(total=total, disable=not progress) as bar, \
+         ProcessPoolExecutor(n_procs) as executor, \
+         outfile.open("w", buffering=1) as f:
+    # fmt: on
+        for output in executor.map(run_radex, *iterables):
             f.write(",".join(output) + "\n")
             bar.update(1)
 
     names = [var.name for var in Vars]
     df = pd.read_csv(outfile, header=None, names=names)
 
     for name in names:
@@ -272,26 +294,26 @@
 
     return dataset.squeeze()
 
 
 # utility functions
 def get_empty_array(
     QN_ul,
-    T_kin=100,
-    N_mol=1e15,
-    n_H2=1e3,
-    n_pH2=None,
-    n_oH2=None,
-    n_e=None,
-    n_H=None,
-    n_He=None,
-    n_Hp=None,
-    T_bg=2.73,
-    dv=1.0,
-    geom="uni",
+    T_kin,
+    N_mol,
+    n_H2,
+    n_pH2,
+    n_oH2,
+    n_e,
+    n_H,
+    n_He,
+    n_Hp,
+    T_bg,
+    dv,
+    geom,
 ):
     """Make an empty xarray.DataArray for storing grid RADEX results."""
     values = {
         Dims.QN_ul: ensure_values(QN_ul),
         Dims.T_kin: ensure_values(T_kin, "K"),
         Dims.N_mol: ensure_values(N_mol, "cm^-2"),
         Dims.n_H2: ensure_values(n_H2, "cm^-3"),
@@ -317,15 +339,15 @@
     freq_lim = lamda.freq_lim
 
     dims, coords = empty.dims, empty.coords
     flatargs = product(*(coords[dim].values for dim in dims))
 
     for args in flatargs:
         kwargs = dict(zip(dims, args))
-        kwargs["id"] = ndradex.utils.random_hex()
+        kwargs["id"] = get_random_hex(8)
         kwargs["freq_lim"] = freq_lim[kwargs["QN_ul"]]
         yield kwargs
 
 
 def get_input_template(lamda, empty):
     """Make template string for RADEX input."""
     n_dims = [
@@ -363,7 +385,12 @@
 
     values = np.asarray(values)
 
     if values.size == 1 and not values.shape:
         return values[np.newaxis]
     else:
         return values
+
+
+def get_random_hex(length: int = 8) -> str:
+    """Return a random hexadecimal string of given length."""
+    return f"{getrandbits(length * 4):x}"
```

### Comparing `ndradex-0.2.2/ndradex/radex.py` & `ndradex-0.3.0/ndradex/radex.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,127 +1,126 @@
 __all__ = []
 
 
 # standard library
 from logging import getLogger
 from pathlib import Path
-from subprocess import PIPE
-from subprocess import run as sprun
+from subprocess import PIPE, run as sprun
 from subprocess import CalledProcessError, TimeoutExpired
+from typing import List, Optional, Sequence, Union
 
 
 # dependencies
-import ndradex
+from .consts import NDRADEX, RADEX_VERSION
+
+
+# type hints
+PathLike = Union[Path, str]
 
 
 # constants
-N_VARS = 10
-ERROR_OUTPUT = ("NaN",) * N_VARS
+N_OUTPUT_VALUES = 10
 
 
+# module logger
 logger = getLogger(__name__)
 
 
-# main function
 def run(
-    input,
-    radex=None,
-    timeout=None,
-    cleanup=True,
-    logfile="radex.log",
-    encoding="utf-8",
-):
-    """Run RADEX and get result as tuple of string.
-
-    Note that this function only reads the last line of RADEX outfile.
-    This means that only the values of the transition at the highest
-    frequency spacified in the RADEX input will be returned.
+    input: Sequence[str],
+    radex: PathLike,
+    cleanup: bool = True,
+    timeout: Optional[float] = None,
+) -> List[str]:
+    """Run RADEX and return the output as a list of strings.
+
+    Note that the function only reads the last line of a RADEX output.
+    This means that the function will only return the values
+    of the highest-frequency transition specified in the RADEX input.
 
     Args:
-        input (str or sequence): RADEX input. See examples below.
-        radex (str or path, optional): RADEX path. If not spacified,
-            then the builtin RADEX with uniform geometry will be used.
-        timeout (int, optional): Timeout of a RADEX run in units of second.
-            Default is None (unlimited run time is permitted).
-        cleanup (bool, optional): If True (default), then the RADEX outfile
-            (e.g. radex.out) and logfile (e.g., radex.log) will be deleted.
-        logfile (str or path, optional): Path of logfile. This is only used
-            for identifying the path of logfile in the cleanup method.
-        encoding (str, optional): File encofing. Default is utf-8.
+        input: Input strings for RADEX. See the examples below.
+        radex: Absolute path of the RADEX binary to be run.
+        cleanup: If True, the RADEX output file will be deleted.
+        timeout: Timeout of the run in units of seconds.
+            Default is None (unlimited run time is allowed).
 
     Returns:
-        output (tuple of str): RADEX output values.
+        RADEX output as a list of strings.
 
     Examples:
-        To get the values of CO(1-0) @ T_kin = 100 K, n_H2 = 1e3 cm^-3,
-        N_CO = 1e15 cm^-2, T_bg = 2.73 K, and dv = 1.0 km s^-1:
+        To get output of CO(1-0) @ T_kin = 100 K, n_H2 = 1e3 cm^-3,
+        N_CO = 1e15 cm^-2, T_bg = 2.73 K, and dv = 1.0 km s^-1::
 
-            >>> input = ['co.dat', 'radex.out', '110 120', '100',
-                        '1', 'H2', '1e3', '2.73', '1e15', '1.0', 0]
-            >>> output = run(input)
+            input = [
+                "co.dat", "radex.out", "110 120", "100",
+                "1", "H2", "1e3", "2.73", "1e15", "1.0", "0",
+            ]
+            output = run(input, "/path/to/radex")
 
     """
-    if radex is None:
-        radex = ndradex.RADEX_BINPATH / "radex-uni"
-
-    try:
-        input, outfile = ensure_input(input, encoding)
-    except (AttributeError, IndexError, TypeError):
-        logger.warning("RADEX did not run due to invalid input")
-        return ERROR_OUTPUT
-
     try:
-        cp = sprun(
-            [radex],
-            input=input,
+        sprun(
+            str(radex),
+            input="\n".join(input),
             timeout=timeout,
             stdout=PIPE,
             stderr=PIPE,
             check=True,
+            text=True,
         )
-        return ensure_output(cp, outfile, encoding)
+        return finalize(input[1], cleanup)
+    except (IndexError, TypeError):
+        logger.warning("RADEX did not run due to invalid input")
+        return ["NaN"] * N_OUTPUT_VALUES
     except FileNotFoundError:
         logger.warning("RADEX path or moldata does not exist")
-        return ERROR_OUTPUT
+        return ["NaN"] * N_OUTPUT_VALUES
     except CalledProcessError:
         logger.warning("RADEX failed due to invalid input")
-        return ERROR_OUTPUT
+        return ["NaN"] * N_OUTPUT_VALUES
     except TimeoutExpired:
         logger.warning("RADEX interrupted due to timeout")
-        return ERROR_OUTPUT
+        return ["NaN"] * N_OUTPUT_VALUES
     except RuntimeError:
         logger.warning("RADEX version is not valid")
-        return ERROR_OUTPUT
-    finally:
-        if cleanup:
-            remove_file(logfile)
-            remove_file(outfile)
-
+        return ["NaN"] * N_OUTPUT_VALUES
 
-# utility functions
-def ensure_input(input, encoding="utf-8"):
-    """Ensure the type of input and the path of outfile."""
-    if isinstance(input, (list, tuple)):
-        outfile = input[1]
-        input = "\n".join(input).encode(encoding)
-    else:
-        outfile = input.split("\n")[1]
-        input = input.encode(encoding)
 
-    return input, outfile
+def build(force: bool = False) -> None:
+    """Build the builtin RADEX binaries."""
+    if force:
+        sprun(
+            args=["make", "clean"],
+            cwd=NDRADEX / "bin",
+            stdout=PIPE,
+            stderr=PIPE,
+            check=True,
+        )
 
+    sprun(
+        args=[
+            "make",
+            "build",
+            "RADEX_LOGFILE=/dev/null",
+            "RADEX_MAXITER=999999",
+        ],
+        cwd=NDRADEX / "bin",
+        stdout=PIPE,
+        stderr=PIPE,
+        check=True,
+    )
 
-def ensure_output(cp, outfile, encoding="utf-8"):
-    """Ensure that the RADEX output is valid."""
-    if ndradex.RADEX_VERSION not in cp.stdout.decode(encoding):
-        raise RuntimeError("RADEX version is not valid")
 
-    with open(outfile, encoding=encoding) as f:
-        return f.readlines()[-1].split()[-N_VARS:]
+def finalize(output: PathLike, cleanup: bool) -> List[str]:
+    """Read a RADEX output file and return the final output."""
+    try:
+        with open(output) as f:
+            lines = f.readlines()
 
+        if RADEX_VERSION not in lines[0]:
+            raise RuntimeError("RADEX version is not valid")
 
-def remove_file(path):
-    """Remove file forcibly (i.e., rm -f <path>)."""
-    try:
-        Path(path).unlink()
-    except FileNotFoundError:
-        pass
+        return lines[-1].split()[-N_OUTPUT_VALUES:]
+    finally:
+        if cleanup:
+            Path(output).unlink(missing_ok=True)
```

