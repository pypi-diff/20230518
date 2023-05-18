# Comparing `tmp/snk-0.6.3.tar.gz` & `tmp/snk-0.6.4.tar.gz`

## Comparing `snk-0.6.3.tar` & `snk-0.6.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.3/Dockerfile
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 snk-0.6.3/mkdocs.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.3/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.3/docs/CNAME
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.3/docs/index.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snk-0.6.3/docs/reference/cli.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.3/docs/reference/errors.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.3/docs/reference/main.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.3/docs/reference/nest.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.3/snk/__about__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.3/snk/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.3/snk/errors.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 snk-0.6.3/snk/main.py
--rw-r--r--   0        0        0    15584 2020-02-02 00:00:00.000000 snk-0.6.3/snk/nest.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.3/snk/pipeline.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.3/snk/cli/__init__.py
--rw-r--r--   0        0        0    16668 2020-02-02 00:00:00.000000 snk-0.6.3/snk/cli/cli.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 snk-0.6.3/snk/cli/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.3/snk/cli/options.py
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 snk-0.6.3/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.3/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.3/tests/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.3/tests/conftest.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.3/tests/test_nest.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.3/tests/test_pipline_cli.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.3/tests/test_snk.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.3/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/.snk
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/cli.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/workflow/Snakefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/workflow/envs/base.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.3/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.3/LICENSE.txt
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 snk-0.6.3/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 snk-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.4/Dockerfile
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 snk-0.6.4/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.4/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.4/docs/CNAME
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.4/docs/index.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snk-0.6.4/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.4/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.4/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.4/docs/reference/nest.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.4/snk/__about__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.4/snk/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.4/snk/errors.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 snk-0.6.4/snk/main.py
+-rw-r--r--   0        0        0    15584 2020-02-02 00:00:00.000000 snk-0.6.4/snk/nest.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.4/snk/pipeline.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.4/snk/cli/__init__.py
+-rw-r--r--   0        0        0    16958 2020-02-02 00:00:00.000000 snk-0.6.4/snk/cli/cli.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 snk-0.6.4/snk/cli/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.4/snk/cli/options.py
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 snk-0.6.4/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.4/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.4/tests/__init__.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.4/tests/conftest.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.4/tests/test_nest.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.4/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.4/tests/test_snk.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.4/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/cli.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/workflow/envs/base.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.4/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.4/LICENSE.txt
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 snk-0.6.4/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 snk-0.6.4/PKG-INFO
```

### Comparing `snk-0.6.3/mkdocs.yml` & `snk-0.6.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/.github/workflows/publish.yml` & `snk-0.6.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/.github/workflows/tests.yml` & `snk-0.6.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/docs/index.md` & `snk-0.6.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/snk/main.py` & `snk-0.6.4/snk/main.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/snk/nest.py` & `snk-0.6.4/snk/nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/snk/pipeline.py` & `snk-0.6.4/snk/pipeline.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/snk/cli/cli.py` & `snk-0.6.4/snk/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import inspect
+import platform
+
 import sys
 import typer
 from pathlib import Path
 from typing import Optional, List, Callable
 import subprocess
 import shutil
 import os
@@ -324,26 +326,29 @@
           verbose (bool): Run pipeline in verbose mode.
           help_snakemake (bool): Print the snakemake help and exit.
         Side Effects:
           Runs the pipeline.
         Examples:
           >>> CLI.run(target='my_target', configfile=Path('/path/to/config.yaml'), resource=[Path('/path/to/resource')], verbose=True)
         """
+        if platform.system() == "Darwin" and platform.processor() == "arm" and not os.environ.get("CONDA_SUBDIR"):
+            os.environ["CONDA_SUBDIR"] = "osx-64"
         self.verbose = verbose
         args = []
         if not cores:
             cores = "all"
         args.extend(
             [
                 "--use-conda",
                 f"--conda-prefix={self.conda_prefix_dir}",
                 f"--cores={cores}",
             ]
         )
-        if self.singularity_prefix_dir:
+        if self.singularity_prefix_dir and "--use-singularity" in ctx.args:
+            # only set prefix if --use-singularity is explicitly called
             args.append(f"--singularity-prefix={self.singularity_prefix_dir}")
         if not self.snakefile.exists():
             raise ValueError("Could not find Snakefile")  # this should occur at install
         else:
             args.append(f"--snakefile={self.snakefile}")
 
         if not configfile:
```

### Comparing `snk-0.6.3/snk/cli/config.py` & `snk-0.6.4/snk/cli/config.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/snk/cli/utils.py` & `snk-0.6.4/snk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/tests/.DS_Store` & `snk-0.6.4/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/tests/conftest.py` & `snk-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/tests/test_nest.py` & `snk-0.6.4/tests/test_nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/tests/test_pipline_cli.py` & `snk-0.6.4/tests/test_pipline_cli.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/tests/test_snk.py` & `snk-0.6.4/tests/test_snk.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/tests/utils.py` & `snk-0.6.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/tests/data/artic_v4.1.bed` & `snk-0.6.4/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/tests/data/config.yaml` & `snk-0.6.4/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/tests/data/cov.fasta` & `snk-0.6.4/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/LICENSE.txt` & `snk-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/README.md` & `snk-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/pyproject.toml` & `snk-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snk-0.6.3/PKG-INFO` & `snk-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snk
-Version: 0.6.3
+Version: 0.6.4
 Project-URL: Documentation, https://github.com/wytamma/snk#readme
 Project-URL: Issues, https://github.com/wytamma/snk/issues
 Project-URL: Source, https://github.com/wytamma/snk
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

