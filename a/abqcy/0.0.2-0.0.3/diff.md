# Comparing `tmp/abqcy-0.0.2.tar.gz` & `tmp/abqcy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abqcy-0.0.2.tar", last modified: Wed May 17 17:02:29 2023, max compression
+gzip compressed data, was "abqcy-0.0.3.tar", last modified: Thu May 18 05:31:05 2023, max compression
```

## Comparing `abqcy-0.0.2.tar` & `abqcy-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:02:29.461502 abqcy-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:02:29.453502 abqcy-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:02:29.453502 abqcy-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 17:02:18.000000 abqcy-0.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-17 17:02:18.000000 abqcy-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-17 17:02:18.000000 abqcy-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-17 17:02:18.000000 abqcy-0.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 17:02:18.000000 abqcy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-17 17:02:29.461502 abqcy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-17 17:02:18.000000 abqcy-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:02:29.457502 abqcy-0.0.2/abqcy/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 17:02:18.000000 abqcy-0.0.2/abqcy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-17 17:02:18.000000 abqcy-0.0.2/abqcy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 17:02:29.000000 abqcy-0.0.2/abqcy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-05-17 17:02:18.000000 abqcy-0.0.2/abqcy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-17 17:02:18.000000 abqcy-0.0.2/abqcy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:02:29.457502 abqcy-0.0.2/abqcy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-17 17:02:29.000000 abqcy-0.0.2/abqcy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-17 17:02:29.000000 abqcy-0.0.2/abqcy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:02:29.000000 abqcy-0.0.2/abqcy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-17 17:02:29.000000 abqcy-0.0.2/abqcy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-17 17:02:29.000000 abqcy-0.0.2/abqcy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 17:02:29.000000 abqcy-0.0.2/abqcy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:02:29.457502 abqcy-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-17 17:02:18.000000 abqcy-0.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-17 17:02:18.000000 abqcy-0.0.2/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-17 17:02:18.000000 abqcy-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-17 17:02:18.000000 abqcy-0.0.2/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-17 17:02:18.000000 abqcy-0.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-17 17:02:18.000000 abqcy-0.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:02:29.457502 abqcy-0.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-17 17:02:18.000000 abqcy-0.0.2/examples/elastic.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:02:29.457502 abqcy-0.0.2/examples/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    14704 2023-05-17 17:02:18.000000 abqcy-0.0.2/examples/templates/umat.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-17 17:02:18.000000 abqcy-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:02:29.461502 abqcy-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:02:29.457502 abqcy-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:02:29.457502 abqcy-0.0.2/tests/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)    42467 2023-05-17 17:02:18.000000 abqcy-0.0.2/tests/inputs/column.inp
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-17 17:02:18.000000 abqcy-0.0.2/tests/run.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:31:05.954115 abqcy-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:31:05.950115 abqcy-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:31:05.950115 abqcy-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-18 05:30:54.000000 abqcy-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-18 05:30:54.000000 abqcy-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-18 05:30:54.000000 abqcy-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-18 05:30:54.000000 abqcy-0.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 05:30:54.000000 abqcy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-18 05:31:05.954115 abqcy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-18 05:30:54.000000 abqcy-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:31:05.950115 abqcy-0.0.3/abqcy/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 05:30:54.000000 abqcy-0.0.3/abqcy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 05:30:54.000000 abqcy-0.0.3/abqcy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 05:31:05.000000 abqcy-0.0.3/abqcy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-18 05:30:54.000000 abqcy-0.0.3/abqcy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-18 05:30:54.000000 abqcy-0.0.3/abqcy/subs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-18 05:30:54.000000 abqcy-0.0.3/abqcy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:31:05.954115 abqcy-0.0.3/abqcy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-18 05:31:05.000000 abqcy-0.0.3/abqcy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 05:31:05.000000 abqcy-0.0.3/abqcy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:31:05.000000 abqcy-0.0.3/abqcy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 05:31:05.000000 abqcy-0.0.3/abqcy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-18 05:31:05.000000 abqcy-0.0.3/abqcy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 05:31:05.000000 abqcy-0.0.3/abqcy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:31:05.954115 abqcy-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-18 05:30:54.000000 abqcy-0.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-18 05:30:54.000000 abqcy-0.0.3/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-18 05:30:54.000000 abqcy-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-18 05:30:54.000000 abqcy-0.0.3/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-18 05:30:54.000000 abqcy-0.0.3/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-18 05:30:54.000000 abqcy-0.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-18 05:30:54.000000 abqcy-0.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:31:05.954115 abqcy-0.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-18 05:30:54.000000 abqcy-0.0.3/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-18 05:30:54.000000 abqcy-0.0.3/examples/elastic.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-18 05:30:54.000000 abqcy-0.0.3/examples/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-18 05:30:54.000000 abqcy-0.0.3/examples/elastic.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:31:05.954115 abqcy-0.0.3/examples/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-18 05:30:54.000000 abqcy-0.0.3/examples/templates/umat.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-05-18 05:30:54.000000 abqcy-0.0.3/examples/templates/umat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-18 05:30:54.000000 abqcy-0.0.3/examples/templates/umat.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-18 05:30:54.000000 abqcy-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 05:31:05.954115 abqcy-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:31:05.954115 abqcy-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:31:05.954115 abqcy-0.0.3/tests/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)    42467 2023-05-18 05:30:54.000000 abqcy-0.0.3/tests/inputs/column.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-18 05:30:54.000000 abqcy-0.0.3/tests/run.bat
```

### Comparing `abqcy-0.0.2/.github/workflows/release.yml` & `abqcy-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.2/.gitignore` & `abqcy-0.0.3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -180,7 +180,10 @@
 *.dat
 *.msg
 *.odb
 *.prt
 *.sim
 *.sta
 jobs/
+
+# temporary autoapi files
+docs/autoapi/
```

### Comparing `abqcy-0.0.2/LICENSE` & `abqcy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.2/PKG-INFO` & `abqcy-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abqcy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Write Abaqus Subroutines in Python
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: GitHub, https://github.com/haiiliin/abqcy/
 Project-URL: PyPI, https://pypi.org/project/abqcy/
 Project-URL: Read the Docs, https://readthedocs.org/projects/abqcy
 Project-URL: Documentation, https://docs.abqcy.com/
 Project-URL: Bug Report, https://github.com/haiiliin/abqcy/issues/
```

### Comparing `abqcy-0.0.2/abqcy/cli.py` & `abqcy-0.0.3/abqcy/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import re
 import shutil
 from pathlib import Path
 
 from abqpy.cli import abaqus
 from Cython.Build import cythonize
 
+from abqcy.subs import subs
+
 
 class AbqcyCLI:
     """The ``abqcy`` command-line interface."""
 
     def compile(
         self,
         script: str,
@@ -72,15 +74,15 @@
             Whether to generate an HTML file with annotations, by default True.
         kwargs
             Additional keyword arguments to pass to the ``cythonize`` function.
         """
         cythonize(script, exclude=exclude, nthreads=nthreads, aliases=aliases, quiet=quiet, force=force,
                   language=language, exclude_failures=exclude_failures, annotate=annotate, **kwargs)  # fmt: skip
         compiled = Path(script).with_suffix(".c")
-        replaced = re.sub("__PYX_EXTERN_C void ", 'extern "C" void ', compiled.read_text())
+        replaced = re.sub(f"(__PYX_EXTERN_C )?void ({'|'.join(subs)})", r'extern "C" void \2', compiled.read_text())
         compiled.write_text(replaced)
         abaqus.abaqus("make", library=str(compiled))
 
     def run(
         self,
         input: str,
         user: str,
@@ -94,33 +96,36 @@
 
         Parameters
         ----------
         input : str
             The path to the input file.
         user : str
             The name of the user subroutine, if it is a Cython/Pure Python script, it will be compiled
-            to an object file automatically.
+            to an object file automatically. If a companion ``.pxd`` file is found, it will be copied.
         job : str, optional
             The name of the job, by default the current directory name.
         output : str, optional
             The path to the output directory, by default the current directory.
         script : str, optional
             The Python script to run after finishing the job to post-process the results.
         kwargs
             Additional keyword arguments to pass to the ``abaqus`` command to make the object file.
         """
         # Prepare the working directory
         output = Path(output or ".").resolve()
         job = job or Path(input).stem
+        user_pxd = Path(user).with_suffix(".pxd")
         if not output.exists():
             output.mkdir(parents=True)
         if not (output / Path(input).name).exists():
             shutil.copy(input, output)
         if not (output / Path(user).name).exists():
             shutil.copy(user, output)
+        if user_pxd.exists() and not (output / user_pxd.name).exists():
+            shutil.copy(user_pxd, output)
         if script and not (output / Path(script).name).exists():
             shutil.copy(script, output)
         os.chdir(output)
 
         # Compile the user subroutine if it is a Cython/Pure Python script
         if user.endswith((".pyx", ".py")):
             self.compile(Path(user).name)
```

### Comparing `abqcy-0.0.2/abqcy/version.py` & `abqcy-0.0.3/abqcy/version.py`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.2/abqcy.egg-info/PKG-INFO` & `abqcy-0.0.3/abqcy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abqcy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Write Abaqus Subroutines in Python
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: GitHub, https://github.com/haiiliin/abqcy/
 Project-URL: PyPI, https://pypi.org/project/abqcy/
 Project-URL: Read the Docs, https://readthedocs.org/projects/abqcy
 Project-URL: Documentation, https://docs.abqcy.com/
 Project-URL: Bug Report, https://github.com/haiiliin/abqcy/issues/
```

### Comparing `abqcy-0.0.2/docs/Makefile` & `abqcy-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.2/docs/cli.md` & `abqcy-0.0.3/docs/cli.md`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.2/docs/conf.py` & `abqcy-0.0.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "sphinx.ext.githubpages",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx_autodoc_typehints",
     "sphinx_copybutton",
     "sphinx_codeautolink",
     "sphinx_design",
+    "sphinx_inline_tabs",
     "sphinxcontrib.programoutput",
     "hoverxref.extension",
     "autoapi.extension",
 ]
 
 # MyST configuration
 myst_enable_extensions = [
```

### Comparing `abqcy-0.0.2/docs/getting-started.md` & `abqcy-0.0.3/docs/getting-started.md`

 * *Files 10% similar despite different names*

```diff
@@ -42,16 +42,23 @@
 C:/Users/Hailin/AppData/Local/Programs/Python/Python310/Lib/site-packages/numpy/core/lib
 C:/Program Files (x86)/Windows Kits/10/Lib/10.0.19041.0/um/x64
 C:/Program Files (x86)/Windows Kits/10/Lib/10.0.19041.0/ucrt/x64
 ```
 
 ## Usage
 
-You can now write your Abaqus subroutine in Cython, simple scripts can be found in the
-[examples](https://github.com/haiiliin/abqcy/tree/main/examples) directory.
+You can now write your Abaqus subroutine in Cython, simple scripts can be found in {doc}`examples`.
+
+```{note}
+In order to not mess up with the Cython declarations, you can add a companion `.pxd` file with the same name as your
+Cython `.py` or `.pyx` file, and put the Cython declarations in it.
+If you are not comfortable with keeping two files, you can just use the `.pyx` file with the Cython declarations.
+
+ See {doc}`examples` for detailed examples.
+```
 
 After you have written your subroutine, you can compile it with the `abqcy` command:
 ```shell
 abqcy compile <path-to-your-subroutine>
 ```
 This will compile your subroutine into a C source file (`.c`) and a C header file (`.h`), and then they will be compiled into an object file (`.obj`)
 that can be used by Abaqus. These files are in the same directory as your subroutine.
```

### Comparing `abqcy-0.0.2/docs/make.bat` & `abqcy-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.2/examples/templates/umat.pyx` & `abqcy-0.0.3/examples/templates/umat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,13 @@
-import cython
-
-
-cdef extern from "<aba_for_c.h>":
-    pass
-
-
-cdef public void umat(
-    stress: cython.p_double, statev: cython.p_double, ddsdde: cython.p_double, sse: cython.p_double,
-    spd: cython.p_double, scd: cython.p_double, rpl: cython.p_double, ddsddt: cython.p_double, drplde: cython.p_double,
-    drpldt: cython.p_double, stran: cython.p_double, dstran: cython.p_double, time: cython.p_double,
-    dtime: cython.p_double, temp: cython.p_double, dtemp: cython.p_double, predef: cython.p_double,
-    dpred: cython.p_double, cmname: cython.p_char, ndi: cython.p_int, nshr: cython.p_int, ntens: cython.p_int,
-    nstatv: cython.p_int, props: cython.p_double, nprops: cython.p_int, coords: cython.p_double, drot: cython.p_double,
-    pnewdt: cython.p_double, celent: cython.p_double, dfgrd0: cython.p_double, dfgrd1: cython.p_double,
-    noel: cython.p_int, npt: cython.p_int, layer: cython.p_int, kspt: cython.p_int, jstep: cython.p_int,
-    kinc: cython.p_int,
-):
+def umat(
+    stress, statev, ddsdde, sse, spd, scd, rpl, ddsddt, drplde, drpldt, stran, dstran,
+    time, dtime, temp, dtemp, predef, dpred, cmname, ndi, nshr, ntens, nstatv, props,
+    nprops, coords, drot, pnewdt, celent, dfgrd0, dfgrd1, noel, npt, layer, kspt,
+    jstep, kinc,
+):  # fmt: skip
     r"""Abaqus UMAT interface for the material model.
 
     Parameters
     ----------
     stress : double[:], shape (ntens,), defined in all situations
         This array is passed in as the stress tensor at the beginning of the increment and must be updated in this
         routine to be the stress tensor at the end of the increment. If you specified initial stresses Initial
```

### Comparing `abqcy-0.0.2/pyproject.toml` & `abqcy-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     "sphinx",
     "sphinx-autoapi",
     "sphinx-autodoc-typehints",
     "sphinx-codeautolink",
     "sphinx-copybutton",
     "sphinx-design",
     "sphinx-hoverxref",
+    "sphinx-inline-tabs",
     "sphinx-rtd-theme",
     "sphinxcontrib-programoutput",
 ]
 
 [project.urls]
 "GitHub" = "https://github.com/haiiliin/abqcy/"
 "PyPI" = "https://pypi.org/project/abqcy/"
```

### Comparing `abqcy-0.0.2/tests/inputs/column.inp` & `abqcy-0.0.3/tests/inputs/column.inp`

 * *Files identical despite different names*

