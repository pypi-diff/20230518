# Comparing `tmp/abqcy-0.0.4.tar.gz` & `tmp/abqcy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abqcy-0.0.4.tar", last modified: Thu May 18 12:51:56 2023, max compression
+gzip compressed data, was "abqcy-0.0.5.tar", last modified: Thu May 18 15:53:54 2023, max compression
```

## Comparing `abqcy-0.0.4.tar` & `abqcy-0.0.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.283550 abqcy-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.275550 abqcy-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.279550 abqcy-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-18 12:51:45.000000 abqcy-0.0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-18 12:51:45.000000 abqcy-0.0.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-18 12:51:45.000000 abqcy-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-18 12:51:45.000000 abqcy-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-18 12:51:45.000000 abqcy-0.0.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 12:51:45.000000 abqcy-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-18 12:51:56.283550 abqcy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-18 12:51:45.000000 abqcy-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.279550 abqcy-0.0.4/abqcy/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 12:51:45.000000 abqcy-0.0.4/abqcy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 12:51:45.000000 abqcy-0.0.4/abqcy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 12:51:56.000000 abqcy-0.0.4/abqcy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-05-18 12:51:45.000000 abqcy-0.0.4/abqcy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-18 12:51:45.000000 abqcy-0.0.4/abqcy/subs.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-18 12:51:45.000000 abqcy-0.0.4/abqcy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.279550 abqcy-0.0.4/abqcy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-18 12:51:56.000000 abqcy-0.0.4/abqcy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-18 12:51:56.000000 abqcy-0.0.4/abqcy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:51:56.000000 abqcy-0.0.4/abqcy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 12:51:56.000000 abqcy-0.0.4/abqcy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-18 12:51:56.000000 abqcy-0.0.4/abqcy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 12:51:56.000000 abqcy-0.0.4/abqcy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.279550 abqcy-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-18 12:51:45.000000 abqcy-0.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-18 12:51:45.000000 abqcy-0.0.4/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-18 12:51:45.000000 abqcy-0.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-18 12:51:45.000000 abqcy-0.0.4/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-18 12:51:45.000000 abqcy-0.0.4/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-18 12:51:45.000000 abqcy-0.0.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-18 12:51:45.000000 abqcy-0.0.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.283550 abqcy-0.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-18 12:51:45.000000 abqcy-0.0.4/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-18 12:51:45.000000 abqcy-0.0.4/examples/elastic.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-18 12:51:45.000000 abqcy-0.0.4/examples/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-18 12:51:45.000000 abqcy-0.0.4/examples/elastic.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.283550 abqcy-0.0.4/examples/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-18 12:51:45.000000 abqcy-0.0.4/examples/templates/umat.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-05-18 12:51:45.000000 abqcy-0.0.4/examples/templates/umat.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-18 12:51:45.000000 abqcy-0.0.4/examples/templates/umat.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-18 12:51:45.000000 abqcy-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:51:56.283550 abqcy-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.283550 abqcy-0.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.283550 abqcy-0.0.4/tests/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)    33058 2023-05-18 12:51:45.000000 abqcy-0.0.4/tests/baseline/test_models.test_model_elastic.png
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 12:51:45.000000 abqcy-0.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.283550 abqcy-0.0.4/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-18 12:51:45.000000 abqcy-0.0.4/tests/models/element-output.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-18 12:51:45.000000 abqcy-0.0.4/tests/models/element-visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-18 12:51:45.000000 abqcy-0.0.4/tests/models/element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.279550 abqcy-0.0.4/tests/outputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.279550 abqcy-0.0.4/tests/outputs/element/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:51:56.283550 abqcy-0.0.4/tests/outputs/element/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-18 12:51:45.000000 abqcy-0.0.4/tests/outputs/element/elastic/U3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-18 12:51:45.000000 abqcy-0.0.4/tests/outputs/element/elastic/U3.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    24039 2023-05-18 12:51:45.000000 abqcy-0.0.4/tests/outputs/element/elastic/U3.png
--rw-r--r--   0 runner    (1001) docker     (123)    22542 2023-05-18 12:51:45.000000 abqcy-0.0.4/tests/outputs/element/elastic/U3.svg
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-18 12:51:45.000000 abqcy-0.0.4/tests/run.bat
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-18 12:51:45.000000 abqcy-0.0.4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 12:51:45.000000 abqcy-0.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.425917 abqcy-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.417916 abqcy-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.421917 abqcy-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-18 15:53:41.000000 abqcy-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-18 15:53:41.000000 abqcy-0.0.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-18 15:53:41.000000 abqcy-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-18 15:53:41.000000 abqcy-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-18 15:53:41.000000 abqcy-0.0.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 15:53:41.000000 abqcy-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-18 15:53:54.425917 abqcy-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-18 15:53:41.000000 abqcy-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.421917 abqcy-0.0.5/abqcy/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 15:53:41.000000 abqcy-0.0.5/abqcy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 15:53:41.000000 abqcy-0.0.5/abqcy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 15:53:54.000000 abqcy-0.0.5/abqcy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-18 15:53:41.000000 abqcy-0.0.5/abqcy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-18 15:53:41.000000 abqcy-0.0.5/abqcy/subs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-18 15:53:41.000000 abqcy-0.0.5/abqcy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.421917 abqcy-0.0.5/abqcy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-18 15:53:54.000000 abqcy-0.0.5/abqcy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-18 15:53:54.000000 abqcy-0.0.5/abqcy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:53:54.000000 abqcy-0.0.5/abqcy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 15:53:54.000000 abqcy-0.0.5/abqcy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-18 15:53:54.000000 abqcy-0.0.5/abqcy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 15:53:54.000000 abqcy-0.0.5/abqcy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.425917 abqcy-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-18 15:53:41.000000 abqcy-0.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-18 15:53:41.000000 abqcy-0.0.5/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-05-18 15:53:41.000000 abqcy-0.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-18 15:53:41.000000 abqcy-0.0.5/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-18 15:53:41.000000 abqcy-0.0.5/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-18 15:53:41.000000 abqcy-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-18 15:53:41.000000 abqcy-0.0.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.425917 abqcy-0.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-18 15:53:41.000000 abqcy-0.0.5/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-18 15:53:41.000000 abqcy-0.0.5/examples/elastic.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-18 15:53:41.000000 abqcy-0.0.5/examples/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-18 15:53:41.000000 abqcy-0.0.5/examples/elastic.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.425917 abqcy-0.0.5/examples/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-18 15:53:41.000000 abqcy-0.0.5/examples/templates/umat.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-05-18 15:53:41.000000 abqcy-0.0.5/examples/templates/umat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-18 15:53:41.000000 abqcy-0.0.5/examples/templates/umat.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-18 15:53:41.000000 abqcy-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:53:54.425917 abqcy-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.425917 abqcy-0.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.425917 abqcy-0.0.5/tests/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    33058 2023-05-18 15:53:41.000000 abqcy-0.0.5/tests/baseline/test_models.test_model_elastic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 15:53:41.000000 abqcy-0.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.425917 abqcy-0.0.5/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-18 15:53:41.000000 abqcy-0.0.5/tests/models/element-output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-18 15:53:41.000000 abqcy-0.0.5/tests/models/element-visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-18 15:53:41.000000 abqcy-0.0.5/tests/models/element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.421917 abqcy-0.0.5/tests/outputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.421917 abqcy-0.0.5/tests/outputs/element/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:54.425917 abqcy-0.0.5/tests/outputs/element/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-18 15:53:41.000000 abqcy-0.0.5/tests/outputs/element/elastic/U3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-18 15:53:41.000000 abqcy-0.0.5/tests/outputs/element/elastic/U3.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    24039 2023-05-18 15:53:41.000000 abqcy-0.0.5/tests/outputs/element/elastic/U3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22542 2023-05-18 15:53:41.000000 abqcy-0.0.5/tests/outputs/element/elastic/U3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-18 15:53:41.000000 abqcy-0.0.5/tests/run.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-18 15:53:41.000000 abqcy-0.0.5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 15:53:41.000000 abqcy-0.0.5/tox.ini
```

### Comparing `abqcy-0.0.4/.github/workflows/release.yml` & `abqcy-0.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/.github/workflows/tests.yml` & `abqcy-0.0.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/.gitignore` & `abqcy-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/LICENSE` & `abqcy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/PKG-INFO` & `abqcy-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abqcy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Write Abaqus Subroutines in Python
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: GitHub, https://github.com/haiiliin/abqcy/
 Project-URL: PyPI, https://pypi.org/project/abqcy/
 Project-URL: Read the Docs, https://readthedocs.org/projects/abqcy
 Project-URL: Documentation, https://docs.abqcy.com/
 Project-URL: Bug Report, https://github.com/haiiliin/abqcy/issues/
```

### Comparing `abqcy-0.0.4/abqcy/cli.py` & `abqcy-0.0.5/abqcy/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,16 +123,16 @@
         replaced = re.sub(pattern, r'extern "C" void \2', compiled.read_text(encoding="utf-8"))
         compiled.write_text(replaced, encoding="utf-8")
         abaqus.abaqus("make", library=str(compiled))
 
     def run(
         self,
         model: str,
-        user: str,
         *,
+        user: str = None,
         job: str = None,
         output: str = None,
         post: str = None,
         visualization: str = None,
         **kwargs,
     ):
         """Run Abaqus jobs.
@@ -152,21 +152,21 @@
         post : str, optional
             The Python script to run after finishing the job to post-process the results. In the output script, a
             placeholder ``{odb}`` will be replaced with the path to the output database file.
         visualization : str, optional
             The Python script to run after finishing the job to visualize the results. Typically, this script will plot
             a figure based on the data saved by the post-processing script.
         kwargs
-            Additional keyword arguments to pass to the ``abaqus`` command to make the object file.
+            Additional keyword arguments to pass to the ``abaqus`` command to run the job.
         """
         # Prepare the working directory
         owd = Path.cwd()
         output = Path(output or ".").resolve()
         job = job or Path(model).stem
-        user_pxd = Path(user).with_suffix(".pxd")
+        user_pxd = Path(user).with_suffix(".pxd") if user else None
 
         # Create the output directory and copy the files
         if not output.exists():
             output.mkdir(parents=True)
         for file in (model, user, user_pxd, post, visualization):
             if file and Path(file).exists() and not (output / Path(file).name).exists():
                 shutil.copy(file, output)
@@ -179,25 +179,25 @@
             for file in output.glob("*.inp"):
                 model = file
                 created = True
                 break
             assert created, f"Failed to create model from {model}."
 
         # Compile the user subroutine if it is a Cython/Pure Python script
-        if user.endswith((".pyx", ".py")):
+        if user and user.endswith((".pyx", ".py")):
             self.compile(Path(user).name)
             compiled = False
             for file in output.glob(f"{Path(user).stem}-*.obj"):
                 user = file
                 compiled = True
                 break
             assert compiled, f"Failed to compile {user} to an object file."
 
         # Run the job
-        inp, user = Path(model).stem, Path(user).stem
+        inp, user = Path(model).stem, Path(user).stem if user else None
         abaqus.abaqus("", job=job, input=inp, user=user, interactive=True, **kwargs)
 
         # Run the post-processing script
         if post is not None:
             odb = None
             post = Path(post).name
             for file in output.glob("*.odb"):
```

### Comparing `abqcy-0.0.4/abqcy/subs.py` & `abqcy-0.0.5/abqcy/subs.py`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/abqcy/version.py` & `abqcy-0.0.5/abqcy/version.py`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/abqcy.egg-info/PKG-INFO` & `abqcy-0.0.5/abqcy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abqcy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Write Abaqus Subroutines in Python
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: GitHub, https://github.com/haiiliin/abqcy/
 Project-URL: PyPI, https://pypi.org/project/abqcy/
 Project-URL: Read the Docs, https://readthedocs.org/projects/abqcy
 Project-URL: Documentation, https://docs.abqcy.com/
 Project-URL: Bug Report, https://github.com/haiiliin/abqcy/issues/
```

### Comparing `abqcy-0.0.4/abqcy.egg-info/SOURCES.txt` & `abqcy-0.0.5/abqcy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/docs/Makefile` & `abqcy-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/docs/cli.md` & `abqcy-0.0.5/docs/cli.md`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/docs/conf.py` & `abqcy-0.0.5/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 from __future__ import annotations
 
+import importlib
 import inspect
 import os
 import sys
 
 import abqcy
 
 # -- Project information -----------------------------------------------------
@@ -162,15 +163,15 @@
 
     modname = info["module"]
     fullname = info["fullname"]
 
     filename = modname.replace(".", "/")
     baseurl = f"https://github.com/haiiliin/abqcy/blob/main/{filename}.py"
 
-    submod = sys.modules.get(modname)
+    submod = importlib.import_module(modname)
     if submod is None:
         return baseurl
 
     obj = submod
     for part in fullname.split("."):
         try:
             obj = getattr(obj, part)
```

### Comparing `abqcy-0.0.4/docs/getting-started.md` & `abqcy-0.0.5/docs/getting-started.md`

 * *Files 26% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 is used (it uses the MSVC `cl` compiler).
 Since the compiled `.c` file requires the Python headers and libraries, `abqcy` will try to find them automatically and
 update the `INCLUDE` and `LIB` environment variables.
 If it fails to find them, you need to update the `INCLUDE` and `LIB` environment variables manually.
 
 ## Usage
 
+### Compile the Subroutine
+
 You can now write your Abaqus subroutine in Cython, simple scripts can be found in {doc}`examples`.
 
 ```{note}
 In order to not mess up with the Cython declarations, you can add a companion `.pxd` file with the same name as your
 Cython `.py` or `.pyx` file, and put the Cython declarations in it.
 If you are not comfortable with keeping two files, you can just use the `.pyx` file with the Cython declarations.
 
@@ -44,9 +46,30 @@
 abqcy compile <path-to-your-subroutine>
 ```
 This will compile your subroutine into a C source file (`.c`) and a C header file (`.h`), and then they will be compiled into an object file (`.obj`)
 that can be used by Abaqus. These files are in the same directory as your subroutine.
 
 Now you can use the subroutine in Abaqus, like:
 ```shell
-abaqus job=Job-1 input=model.inp user=your-subroutine.obj
+abaqus job=Job-1 input=<model.inp> user=<subroutine> 
+```
+
+### Run an Abaqus Job, Post-process and Visualize the Results in a Single Command
+
+You can use the `abqcy run` command to run an Abaqus job with your subroutine, post-process the results and visualize
+them in a single command:
+```shell
+abqcy run <script-or-inp> --user=<subroutine> --job=<job-name> --output=<output-dir> --post=<post-process-script> --visualization=<visualization-script>
 ```
+where:
+
+- `script-or-inp`: a Python script (`.py`) file using the `abaqus cae` command to create the input file (`.inp`) or
+  an input file (`.inp`) to run.
+- `subroutine`: a Cython/Python file (`py` or `pyx`) or any other file that can be used by Abaqus as a user subroutine
+  (`.f`, `.for`, `.c`, `.cc`, `.cpp`, `.cxx`). When using a Cython/Python file, the `abqcy compile` command will be used to 
+  compile it into an object file (`.obj`) before running the job.
+- `job-name`: the name of the job to run. Defaults to the name of the input file.
+- `output-dir`: the directory to store all the output files including models, subroutines, scripts, results, etc.
+  Defaults to the current working directory.
+- `post-process-script`: a Python script (`.py`) file to post-process the results using the `abaqus cae` command.
+- `visualization-script`: a Python script (`.py`) file to visualize the results executed by the current Python
+  interpreter.
```

### Comparing `abqcy-0.0.4/docs/index.md` & `abqcy-0.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/docs/make.bat` & `abqcy-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/examples/elastic.pxd` & `abqcy-0.0.5/examples/elastic.pxd`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/examples/elastic.pyx` & `abqcy-0.0.5/examples/elastic.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+import cython
+
+
 cdef extern from "<aba_for_c.h>":
     pass
 
 
+@cython.infer_types(True)
 cdef extern void umat(
     double *stress, double *statev, double *ddsdde, double *sse, double *spd,
     double *scd, double *rpl, double *ddsddt, double *drplde, double *drpldt,
     double *stran, double *dstran, double *time, double *dtime, double *temp,
     double *dtemp, double *predef, double *dpred, char *cmname, int *ndi,
     int *nshr, int *ntens, int *nstatv, double *props, int *nprops, double *coords,
     double *drot, double *pnewdt, double *celent, double *dfgrd0, double *dfgrd1,
     int *noel, int *npt, int *layer, int *kspt, int *jstep, int *kinc,
 ):
-    cdef double E, nu, lam, G
     E, nu = props[0], props[1]
     lam = E * nu / ((1.0 + nu) * (1.0 - 2.0 * nu))
     G = E / (2.0 * (1.0 + nu))
 
-    cdef int i, j
     for i in range(3):
         for j in range(3):
             ddsdde[6 * i + j] = lam
         ddsdde[6 * i + i] += 2.0 * G
         ddsdde[6 * (i + 3) + (i + 3)] = G
     for i in range(6):
         for j in range(6):
```

### Comparing `abqcy-0.0.4/examples/templates/umat.pxd` & `abqcy-0.0.5/examples/templates/umat.pxd`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/examples/templates/umat.py` & `abqcy-0.0.5/examples/templates/umat.py`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/examples/templates/umat.pyx` & `abqcy-0.0.5/examples/templates/umat.pyx`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/pyproject.toml` & `abqcy-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/tests/baseline/test_models.test_model_elastic.png` & `abqcy-0.0.5/tests/baseline/test_models.test_model_elastic.png`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/tests/conftest.py` & `abqcy-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/tests/models/element-output.py` & `abqcy-0.0.5/tests/models/element-output.py`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/tests/models/element.py` & `abqcy-0.0.5/tests/models/element.py`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/tests/outputs/element/elastic/U3.csv` & `abqcy-0.0.5/tests/outputs/element/elastic/U3.csv`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/tests/outputs/element/elastic/U3.pdf` & `abqcy-0.0.5/tests/outputs/element/elastic/U3.pdf`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/tests/outputs/element/elastic/U3.png` & `abqcy-0.0.5/tests/outputs/element/elastic/U3.png`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/tests/outputs/element/elastic/U3.svg` & `abqcy-0.0.5/tests/outputs/element/elastic/U3.svg`

 * *Files identical despite different names*

### Comparing `abqcy-0.0.4/tests/test_models.py` & `abqcy-0.0.5/tests/test_models.py`

 * *Files identical despite different names*

