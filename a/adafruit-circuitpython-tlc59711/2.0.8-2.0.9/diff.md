# Comparing `tmp/adafruit-circuitpython-tlc59711-2.0.8.tar.gz` & `tmp/adafruit-circuitpython-tlc59711-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tlc59711-2.0.8.tar", last modified: Fri Aug 26 02:26:07 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-tlc59711-2.0.9.tar", last modified: Mon Dec 19 15:56:09 2022, max compression
```

## Comparing `adafruit-circuitpython-tlc59711-2.0.8.tar` & `adafruit-circuitpython-tlc59711-2.0.9.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:07.692112 adafruit-circuitpython-tlc59711-2.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:07.688112 adafruit-circuitpython-tlc59711-2.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:07.692112 adafruit-circuitpython-tlc59711-2.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:07.692112 adafruit-circuitpython-tlc59711-2.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16275 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:07.692112 adafruit-circuitpython-tlc59711-2.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3332 2022-08-26 02:26:07.692112 adafruit-circuitpython-tlc59711-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2546 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:07.692112 adafruit-circuitpython-tlc59711-2.0.8/adafruit_circuitpython_tlc59711.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3332 2022-08-26 02:26:07.000000 adafruit-circuitpython-tlc59711-2.0.8/adafruit_circuitpython_tlc59711.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-26 02:26:07.000000 adafruit-circuitpython-tlc59711-2.0.8/adafruit_circuitpython_tlc59711.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:26:07.000000 adafruit-circuitpython-tlc59711-2.0.8/adafruit_circuitpython_tlc59711.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-26 02:26:07.000000 adafruit-circuitpython-tlc59711-2.0.8/adafruit_circuitpython_tlc59711.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-26 02:26:07.000000 adafruit-circuitpython-tlc59711-2.0.8/adafruit_circuitpython_tlc59711.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    38536 2022-08-26 02:26:00.000000 adafruit-circuitpython-tlc59711-2.0.8/adafruit_tlc59711.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:07.692112 adafruit-circuitpython-tlc59711-2.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:07.692112 adafruit-circuitpython-tlc59711-2.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5579 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:07.692112 adafruit-circuitpython-tlc59711-2.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    11876 2022-08-26 02:26:00.000000 adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_dev.py
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-08-26 02:26:00.000000 adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_fancyled.py
--rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-08-26 02:26:00.000000 adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_fastset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-08-26 02:26:00.000000 adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-08-26 02:26:00.000000 adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_singlechip_autoshow.py
--rw-r--r--   0 runner    (1001) docker     (121)     3300 2022-08-26 02:26:00.000000 adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_test_bcdata.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-08-26 02:26:00.000000 adafruit-circuitpython-tlc59711-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-26 02:25:53.000000 adafruit-circuitpython-tlc59711-2.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:26:07.692112 adafruit-circuitpython-tlc59711-2.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:56:09.452269 adafruit-circuitpython-tlc59711-2.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:56:09.448269 adafruit-circuitpython-tlc59711-2.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:56:09.448269 adafruit-circuitpython-tlc59711-2.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:56:09.448269 adafruit-circuitpython-tlc59711-2.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:56:09.452269 adafruit-circuitpython-tlc59711-2.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2022-12-19 15:56:09.452269 adafruit-circuitpython-tlc59711-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:56:09.452269 adafruit-circuitpython-tlc59711-2.0.9/adafruit_circuitpython_tlc59711.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2022-12-19 15:56:09.000000 adafruit-circuitpython-tlc59711-2.0.9/adafruit_circuitpython_tlc59711.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2022-12-19 15:56:09.000000 adafruit-circuitpython-tlc59711-2.0.9/adafruit_circuitpython_tlc59711.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 15:56:09.000000 adafruit-circuitpython-tlc59711-2.0.9/adafruit_circuitpython_tlc59711.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-19 15:56:09.000000 adafruit-circuitpython-tlc59711-2.0.9/adafruit_circuitpython_tlc59711.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-19 15:56:09.000000 adafruit-circuitpython-tlc59711-2.0.9/adafruit_circuitpython_tlc59711.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39396 2022-12-19 15:56:00.000000 adafruit-circuitpython-tlc59711-2.0.9/adafruit_tlc59711.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:56:09.452269 adafruit-circuitpython-tlc59711-2.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:56:09.452269 adafruit-circuitpython-tlc59711-2.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 15:56:09.452269 adafruit-circuitpython-tlc59711-2.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2022-12-19 15:56:00.000000 adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2022-12-19 15:56:00.000000 adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_fancyled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2022-12-19 15:56:00.000000 adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_fastset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2022-12-19 15:56:00.000000 adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2022-12-19 15:56:00.000000 adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_singlechip_autoshow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2022-12-19 15:56:00.000000 adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_test_bcdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2022-12-19 15:56:00.000000 adafruit-circuitpython-tlc59711-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-19 15:55:48.000000 adafruit-circuitpython-tlc59711-2.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 15:56:09.452269 adafruit-circuitpython-tlc59711-2.0.9/setup.cfg
```

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tlc59711-2.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/.gitignore` & `adafruit-circuitpython-tlc59711-2.0.9/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-tlc59711-2.0.9/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.15.5
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/.pylintrc` & `adafruit-circuitpython-tlc59711-2.0.9/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tlc59711-2.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/LICENSE` & `adafruit-circuitpython-tlc59711-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tlc59711-2.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-tlc59711-2.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tlc59711-2.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/PKG-INFO` & `adafruit-circuitpython-tlc59711-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tlc59711
-Version: 2.0.8
+Version: 2.0.9
 Summary: CircuitPython library for TLC59711 16-bit 12 channel LED PWM driver.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TLC59711
 Keywords: adafruit,tlc59711,16-bit,12-channel,led,pwm,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/README.rst` & `adafruit-circuitpython-tlc59711-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/adafruit_circuitpython_tlc59711.egg-info/PKG-INFO` & `adafruit-circuitpython-tlc59711-2.0.9/adafruit_circuitpython_tlc59711.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tlc59711
-Version: 2.0.8
+Version: 2.0.9
 Summary: CircuitPython library for TLC59711 16-bit 12 channel LED PWM driver.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TLC59711
 Keywords: adafruit,tlc59711,16-bit,12-channel,led,pwm,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/adafruit_circuitpython_tlc59711.egg-info/SOURCES.txt` & `adafruit-circuitpython-tlc59711-2.0.9/adafruit_circuitpython_tlc59711.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 optional_requirements.txt
 pylama.ini
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_tlc59711.egg-info/PKG-INFO
 adafruit_circuitpython_tlc59711.egg-info/SOURCES.txt
 adafruit_circuitpython_tlc59711.egg-info/dependency_links.txt
 adafruit_circuitpython_tlc59711.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/adafruit_tlc59711.py` & `adafruit-circuitpython-tlc59711-2.0.9/adafruit_tlc59711.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 * The API is mostly compatible to the DotStar / NeoPixel Libraries
     and is therefore also compatible with FancyLED.
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 """
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_TLC59711.git"
 
 
 # pylint - globally disable
 # 'invalid-name' check to allow for datasheet conform short channel and register names.
 # pylint: disable=invalid-name
 # 'too-many-lines' with the extra class and the api backwards compatibel things i have ~1100 lines..
@@ -45,14 +45,19 @@
 # pylint: disable=too-many-lines
 
 
 import struct
 
 from micropython import const
 
+try:
+    from typing import Dict, List, Optional, Tuple
+    from busio import SPI
+except ImportError:
+    pass
 
 _CHIP_BUFFER_BYTE_COUNT = const(28)
 
 COLORS_PER_PIXEL = const(3)
 PIXEL_PER_CHIP = const(4)
 CHANNEL_PER_CHIP = const(COLORS_PER_PIXEL * PIXEL_PER_CHIP)
 
@@ -170,19 +175,19 @@
 
     The TLC59711 & TLC5971 chip is designed to drive 4 RGB LEDs with 16-bit PWM per Color.
     This Library can control 1..many chips.
     The class has an interface compatible with the FancyLED library -
     and the API is similar to the NeoPixel and DotStar Interfaces.
 
     :param ~busio.SPI spi: An instance of the SPI bus connected to the chip.
-        The clock and MOSI/outout must be set, the MISO/input is unused.
-        Maximal data clock frequence is:
+        The clock and MOSI/output must be set, the MISO/input is unused.
+        Maximal data clock frequency is:
         - TLC59711: 10MHz
         - TLC5971: 20MHz
-    :param bool pixel_count: Number of RGB-LEDs (=Pixels) that are connected. (default=4)
+    :param int pixel_count: Number of RGB-LEDs (=Pixels) that are connected. (default=4)
     """
 
     # pylint: disable=too-many-instance-attributes
     # it just does make senes to have the chip params as attributes.
 
     # """
     # TLC5971 data / register structure
@@ -269,15 +274,15 @@
     #     v &= ~mask
     #     if x:
     #         # If x was True, set the bit indicated by the mask.
     #         v |= mask
     #     # Return the result, we're done.
     #     return v
 
-    def __init__(self, spi, *, pixel_count=4):
+    def __init__(self, spi: SPI, *, pixel_count: int = 4) -> None:
         """Init."""
         self._spi = spi
         self.pixel_count = pixel_count
         self.channel_count = self.pixel_count * COLORS_PER_PIXEL
         # calculate how many chips are connected
         self.chip_count = self.pixel_count // 4
 
@@ -303,24 +308,29 @@
         self.blank = False
 
         # preparation done → now initialize buffer to default values
         self._init_buffer()
         self._buffer_index_lookuptable = []
         self._init_lookuptable()
 
-    def _init_buffer(self):
+    def _init_buffer(self) -> None:
         for chip_index in range(self.chip_count):
             # set Write Command (6Bit) WRCMD (fixed: 25h)
             self.chip_set_BCData(chip_index, bcr=self.bcr, bcg=self.bcg, bcb=self.bcb)
             self._chip_set_FunctionControl(chip_index)
             self._chip_set_WriteCommand(chip_index)
 
     def set_chipheader_bits_in_buffer(
-        self, *, chip_index=0, part_bit_offset=0, field=None, value=0
-    ):
+        self,
+        *,
+        chip_index: int = 0,
+        part_bit_offset: int = 0,
+        field: Optional[Dict[str, int]] = None,
+        value: int = 0,
+    ) -> None:
         """Set chip header bits in buffer."""
         if field is None:
             field = {"mask": 0, "length": 0, "offset": 0}
         offset = part_bit_offset + field["offset"]
         # restrict value
         value &= field["mask"]
         # move value to position
@@ -337,15 +347,17 @@
         # set
         header |= value
         # write header back
         struct.pack_into(">I", self._buffer, header_start, header)
 
     ##########################################
 
-    def chip_set_BCData(self, chip_index, bcr=127, bcg=127, bcb=127):
+    def chip_set_BCData(
+        self, chip_index: int, bcr: int = 127, bcg: int = 127, bcb: int = 127
+    ) -> None:
         """
         Set BC-Data.
 
         :param int chip_index: Index of Chip to set.
         :param int bcr: 7-bit value from 0-127 (default=127)
         :param int bcg: 7-bit value from 0-127 (default=127)
         :param int bcb: 7-bit value from 0-127 (default=127)
@@ -366,24 +378,24 @@
         self.set_chipheader_bits_in_buffer(
             chip_index=chip_index,
             part_bit_offset=_BC_CHIP_BUFFER_BIT_OFFSET,
             field=_BC_FIELDS["BCB"],
             value=bcb,
         )
 
-    def update_BCData(self):
+    def update_BCData(self) -> None:
         """
         Update BC-Data for all Chips in Buffer.
 
         need to be called after you changed on of the BC-Data Parameters. (bcr, bcg, bcb)
         """
         for chip_index in range(self.chip_count):
             self.chip_set_BCData(chip_index, bcr=self.bcr, bcg=self.bcg, bcb=self.bcb)
 
-    def _chip_set_FunctionControl(self, chip_index):
+    def _chip_set_FunctionControl(self, chip_index: int) -> None:
         """
         Set Function Control Bits in Buffer.
 
         values from object global parameters are used.
 
         :param int chip_index: Index of Chip to set.
         """
@@ -415,114 +427,116 @@
         self.set_chipheader_bits_in_buffer(
             chip_index=chip_index,
             part_bit_offset=_FC_CHIP_BUFFER_BIT_OFFSET,
             field=_FC_FIELDS["BLANK"],
             value=self.blank,
         )
 
-    def update_fc(self):
+    def update_fc(self) -> None:
         """
         Update Function Control Bits for all Chips in Buffer.
 
         need to be called after you changed on of the Function Control Bit Parameters.
         (outtmg, extgck, tmgrst, dsprpt, blank)
         """
         for chip_index in range(self.chip_count):
             self._chip_set_FunctionControl(chip_index)
 
-    def _chip_set_WriteCommand(self, chip_index):
+    def _chip_set_WriteCommand(self, chip_index: int) -> None:
         """Set WRITE_COMMAND."""
         # set all bits
         self.set_chipheader_bits_in_buffer(
             chip_index=chip_index,
             part_bit_offset=_WC_CHIP_BUFFER_BIT_OFFSET,
             field=_WC_FIELDS["WRITE_COMMAND"],
             value=WRITE_COMMAND,
         )
 
-    def _init_lookuptable(self):
+    def _init_lookuptable(self) -> None:
         for channel_index in range(self.channel_count):
             buffer_index = (_CHIP_BUFFER_BYTE_COUNT // _BUFFER_BYTES_PER_COLOR) * (
                 channel_index // CHANNEL_PER_CHIP
             ) + channel_index % CHANNEL_PER_CHIP
             buffer_index *= _BUFFER_BYTES_PER_COLOR
             buffer_index += _CHIP_BUFFER_HEADER_BYTE_COUNT
             self._buffer_index_lookuptable.append(buffer_index)
 
     ##########################################
 
-    def _write(self):
+    def _write(self) -> None:
         # Write out the current state to the shift register.
         try:
             # Lock the SPI bus and configure it for the shift register.
             while not self._spi.try_lock():
                 pass
             self._spi.configure(baudrate=self._spi.frequency, polarity=0, phase=0)
             self._spi.write(self._buffer)
         finally:
             # Ensure the SPI bus is unlocked.
             self._spi.unlock()
 
-    def show(self):
+    def show(self) -> None:
         """Write out the current LED PWM state to the chip."""
         self._write()
 
     ##########################################
 
     @staticmethod
-    def calculate_Ioclmax(*, Riref=2.48):
+    def calculate_Ioclmax(*, Riref: float = 2.48) -> float:
         """
         Calculate Maximum Constant Sink Current Value.
 
         see:
         8.4.1 Maximum Constant Sink Current Setting
         http://www.ti.com/lit/ds/symlink/tlc5971.pdf#page=18&zoom=160,0,524
 
         Riref = (Viref / Ioclmax) * 41
         Ioclmax = (41 / Riref) * Viref
 
         :param float Riref: resistor value (kΩ) (default=20)
-        :return tuple: Ioclmax (mA)
+        :return float: Ioclmax (mA)
         """
         # Riref                 = (Viref / Ioclmax) * 41    | / 41
         # Riref / 41            = Viref / Ioclmax           | switch
         # 41 / Riref            = Ioclmax / Viref           | * Viref
         # (41 / Riref) * Viref  = Ioclmax
         if not 0.8 <= Riref <= 24.8:
-            raise ValueError("Riref {} not in range: 0.8kΩ..25kΩ".format(Riref))
+            raise ValueError(f"Riref {Riref} not in range: 0.8kΩ..25kΩ")
         Viref = 1.21
         Ioclmax = (41 / Riref) * Viref
         if not 2.0 <= Ioclmax <= 60.0:
-            raise ValueError("Ioclmax {} not in range: 2mA..60mA".format(Ioclmax))
+            raise ValueError(f"Ioclmax {Ioclmax} not in range: 2mA..60mA")
         return Ioclmax
 
     @staticmethod
-    def calculate_Riref(*, Ioclmax=20):
+    def calculate_Riref(*, Ioclmax: float = 20) -> float:
         """
         Calculate Maximum Constant Sink Current Value.
 
         see:
         8.4.1 Maximum Constant Sink Current Setting
         http://www.ti.com/lit/ds/symlink/tlc5971.pdf#page=19&zoom=200,0,697
 
         Riref = (Viref / Ioclmax) * 41
 
         :param float Ioclmax: target max output current (mA) (default=20)
-        :return tuple: Riref (kΩ)
+        :return float: Riref (kΩ)
         """
         if not 2.0 <= Ioclmax <= 60.0:
-            raise ValueError("Ioclmax {} not in range: 2mA..60mA".format(Ioclmax))
+            raise ValueError(f"Ioclmax {Ioclmax} not in range: 2mA..60mA")
         Viref = 1.21
         Riref = (Viref / Ioclmax) * 41
         if not 0.8 <= Riref <= 24.8:
-            raise ValueError("Riref {} not in range: 0.8kΩ..25kΩ".format(Riref))
+            raise ValueError(f"Riref {Riref} not in range: 0.8kΩ..25kΩ")
         return Riref
 
     @staticmethod
-    def calculate_BCData(*, Ioclmax=18, IoutR=17, IoutG=15, IoutB=9):
+    def calculate_BCData(
+        *, Ioclmax: float = 18, IoutR: float = 17, IoutG: float = 15, IoutB: float = 9
+    ) -> Tuple[float, float, float]:
         """
         Calculate Global Brightness Control Values.
 
         see:
         8.5.1 Global Brightness Control (BC) Function (Sink Current Control)
         http://www.ti.com/lit/ds/symlink/tlc5971.pdf#page=19&zoom=200,0,697
 
@@ -538,52 +552,52 @@
             (default=17)
         :return tuple: (bcr, bcg, bcb)
         """
         # Iout                 =  Ioclmax * (BCX / 127)  | / Ioclmax
         # Iout / Ioclmax       =  BCX / 127              | * 127
         # Iout / Ioclmax * 127 =  BCX
         if not 2.0 <= Ioclmax <= 60.0:
-            raise ValueError("Ioclmax {} not in range: 2mA..60mA" "".format(Ioclmax))
+            raise ValueError(f"Ioclmax {Ioclmax} not in range: 2mA..60mA")
         if not 0.0 <= IoutR <= Ioclmax:
-            raise ValueError("IoutR {} not in range: 2mA..{}mA".format(IoutR, Ioclmax))
+            raise ValueError(f"IoutR {IoutR} not in range: 2mA..{Ioclmax}mA")
         if not 0.0 <= IoutG <= Ioclmax:
-            raise ValueError("IoutG {} not in range: 2mA..{}mA".format(IoutG, Ioclmax))
+            raise ValueError(f"IoutG {IoutG} not in range: 2mA..{Ioclmax}mA")
         if not 0.0 <= IoutB <= Ioclmax:
-            raise ValueError("IoutB {} not in range: 2mA..{}mA".format(IoutB, Ioclmax))
+            raise ValueError(f"IoutB {IoutB} not in range: 2mA..{Ioclmax}mA")
         bcr = int((IoutR / Ioclmax) * 127)
         bcg = int((IoutG / Ioclmax) * 127)
         bcb = int((IoutB / Ioclmax) * 127)
         if not 0 <= bcr <= 127:
-            raise ValueError("bcr {} not in range: 0..127".format(bcr))
+            raise ValueError(f"bcr {bcr} not in range: 0..127")
         if not 0 <= bcg <= 127:
-            raise ValueError("bcg {} not in range: 0..127".format(bcg))
+            raise ValueError(f"bcg {bcg} not in range: 0..127")
         if not 0 <= bcb <= 127:
-            raise ValueError("bcb {} not in range: 0..127".format(bcb))
+            raise ValueError(f"bcb {bcb} not in range: 0..127")
         return (bcr, bcg, bcb)
 
     ##########################################
 
     @staticmethod
-    def _convert_01_float_to_16bit_integer(value):
+    def _convert_01_float_to_16bit_integer(value: float) -> int:
         """Convert 0..1 Float Value to 16bit (0..65535) Range."""
         # check if value is in range
-        if not 0.0 <= value[0] <= 1.0:
-            raise ValueError("value[0] {} not in range: 0..1".format(value[0]))
+        if not 0.0 <= value <= 1.0:
+            raise ValueError(f"value[0] {value} not in range: 0..1")
         # convert to 16bit value
         return int(value * 65535)
 
     @classmethod
-    def _convert_if_float(cls, value):
+    def _convert_if_float(cls, value: float) -> int:
         """Convert if value is Float."""
         if isinstance(value, float):
             value = cls._convert_01_float_to_16bit_integer(value)
         return value
 
     @staticmethod
-    def _check_and_convert(value):
+    def _check_and_convert(value: List[int]):
         # loop
         # mega slow
         # for i, val in enumerate(value):
         #     # check if we have float values
         #     if isinstance(val, float):
         #         # check if val is in range
         #         if not 0.0 <= val <= 1.0:
@@ -597,42 +611,44 @@
         #                 "value[{}] {} not in range: 0..65535".format(i, val))
         # discreet is way faster
         # (compared with tlc59711_multi_dev.py: pixels.set_all_black())
         # check if we have float values
         if isinstance(value[0], float):
             # check if value is in range
             if not 0.0 <= value[0] <= 1.0:
-                raise ValueError("value[0] {} not in range: 0..1".format(value[0]))
+                raise ValueError(f"value[0] {value[0]} not in range: 0..1")
             # convert to 16bit value
             value[0] = int(value[0] * 65535)
         else:
             if not 0 <= value[0] <= 65535:
-                raise ValueError("value[0] {} not in range: 0..65535".format(value[0]))
+                raise ValueError(f"value[0] {value[0]} not in range: 0..65535")
         if isinstance(value[1], float):
             if not 0.0 <= value[1] <= 1.0:
-                raise ValueError("value[1] {} not in range: 0..1".format(value[1]))
+                raise ValueError(f"value[1] {value[1]} not in range: 0..1")
             value[1] = int(value[1] * 65535)
         else:
             if not 0 <= value[1] <= 65535:
-                raise ValueError("value[1] {} not in range: 0..65535".format(value[1]))
+                raise ValueError(f"value[1] {value[1]} not in range: 0..65535")
         if isinstance(value[2], float):
             if not 0.0 <= value[2] <= 1.0:
-                raise ValueError("value[2] {} not in range: 0..1".format(value[2]))
+                raise ValueError(f"value[2] {value[2]} not in range: 0..1")
             value[2] = int(value[2] * 65535)
         else:
             if not 0 <= value[2] <= 65535:
-                raise ValueError("value[2] {} not in range: 0..65535".format(value[2]))
+                raise ValueError(f"value[2] {value[2]} not in range: 0..65535")
 
     ##########################################
 
     def _get_channel_16bit_value(self, channel_index):
         buffer_start = self._buffer_index_lookuptable[channel_index]
         return struct.unpack_from(">H", self._buffer, buffer_start)[0]
 
-    def set_pixel_16bit_value(self, pixel_index, value_r, value_g, value_b):
+    def set_pixel_16bit_value(
+        self, pixel_index: int, value_r: int, value_g: int, value_b: int
+    ) -> None:
         """
         Set the value for pixel.
 
         This is a Fast UNPROTECTED function:
         no error / range checking is done.
 
         :param int pixel_index: 0..(pixel_count)
@@ -656,15 +672,17 @@
         self._buffer[buffer_start + 0] = (value_g >> 8) & 0xFF
         self._buffer[buffer_start + 1] = value_g & 0xFF
         buffer_start = self._buffer_index_lookuptable[pixel_start + 2]
         # struct.pack_into('>H', self._buffer, buffer_start, value_r)
         self._buffer[buffer_start + 0] = (value_r >> 8) & 0xFF
         self._buffer[buffer_start + 1] = value_r & 0xFF
 
-    def set_pixel_float_value(self, pixel_index, value_r, value_g, value_b):
+    def set_pixel_float_value(
+        self, pixel_index: int, value_r: int, value_g: int, value_b: int
+    ) -> None:
         """
         Set the value for pixel.
 
         This is a Fast UNPROTECTED function:
         no error / range checking is done.
 
         :param int pixel_index: 0..(pixel_count)
@@ -690,15 +708,17 @@
         buffer_start = self._buffer_index_lookuptable[pixel_start + 1]
         self._buffer[buffer_start + 0] = (value_g >> 8) & 0xFF
         self._buffer[buffer_start + 1] = value_g & 0xFF
         buffer_start = self._buffer_index_lookuptable[pixel_start + 2]
         self._buffer[buffer_start + 0] = (value_r >> 8) & 0xFF
         self._buffer[buffer_start + 1] = value_r & 0xFF
 
-    def set_pixel_16bit_color(self, pixel_index, color):
+    def set_pixel_16bit_color(
+        self, pixel_index: int, color: Tuple[int, int, int]
+    ) -> None:
         """
         Set color for pixel.
 
         This is a Fast UNPROTECTED function:
         no error / range checking is done.
         its a little bit slower as `set_pixel_16bit_value`
 
@@ -721,21 +741,23 @@
         buffer_start = self._buffer_index_lookuptable[pixel_start + 1]
         self._buffer[buffer_start + 0] = (color[1] >> 8) & 0xFF
         self._buffer[buffer_start + 1] = color[1] & 0xFF
         buffer_start = self._buffer_index_lookuptable[pixel_start + 2]
         self._buffer[buffer_start + 0] = (color[0] >> 8) & 0xFF
         self._buffer[buffer_start + 1] = color[0] & 0xFF
 
-    def set_pixel_float_color(self, pixel_index, color):
+    def set_pixel_float_color(
+        self, pixel_index: int, color: Tuple[float, float, float]
+    ) -> None:
         """
         Set color for pixel.
 
         This is a Fast UNPROTECTED function:
         no error / range checking is done.
-        its a little bit slower as `set_pixel_16bit_value`
+        it's a little bit slower as `set_pixel_16bit_value`
 
         :param int pixel_index: 0..(pixel_count)
         :param tuple/float color: 3-tuple of R, G, B;  0..1
         """
         # self.set_pixel_16bit_value(
         #     pixel_index,
         #     int(color[0] * 65535),
@@ -754,34 +776,38 @@
         buffer_start = self._buffer_index_lookuptable[pixel_start + 1]
         self._buffer[buffer_start + 0] = (color[1] >> 8) & 0xFF
         self._buffer[buffer_start + 1] = color[1] & 0xFF
         buffer_start = self._buffer_index_lookuptable[pixel_start + 2]
         self._buffer[buffer_start + 0] = (color[0] >> 8) & 0xFF
         self._buffer[buffer_start + 1] = color[0] & 0xFF
 
-    def set_pixel(self, pixel_index, value):
+    def set_pixel(
+        self,
+        pixel_index: int,
+        value: Tuple[float, float, float],
+    ) -> None:
         """
         Set the R, G, B values for the pixel.
 
-        this funciton hase some advanced error checking.
+        this function hase some advanced error checking.
         it is much slower than the other provided 'bare' variants..
         but therefor gives clues to what is going wrong.. ;-)
 
         :param int pixel_index: 0..(pixel_count)
         :param tuple value: 3-tuple of R, G, B;
             each int 0..65535 or float 0..1
         """
         if 0 <= pixel_index < self.pixel_count:
             # convert to list
             value = list(value)
             # repr(value)
             if len(value) != COLORS_PER_PIXEL:
                 raise IndexError(
-                    "length of value {} does not match COLORS_PER_PIXEL (= {})"
-                    "".format(len(value), COLORS_PER_PIXEL)
+                    f"length of value {len(value)} does not match COLORS_PER_PIXEL"
+                    " (= {COLORS_PER_PIXEL})"
                 )
             # tested:
             # splitting up into variables to not need the list..
             # this is about 0.25ms slower..
             # value_r = value[0]
             # value_g = value[1]
             # value_b = value[2]
@@ -803,46 +829,48 @@
             # buffer_start = self._buffer_index_lookuptable[pixel_start + 2]
             # self._buffer[buffer_start + 0] = (value[0] >> 8) & 0xFF
             # self._buffer[buffer_start + 1] = value[0] & 0xFF
             # simpliefy code
             self.set_pixel_16bit_value(pixel_index, value[0], value[1], value[2])
         else:
             raise IndexError(
-                "index {} out of range [0..{}]" "".format(pixel_index, self.pixel_count)
+                f"index {pixel_index} out of range [0..{self.pixel_count}]"
             )
 
-    def set_pixel_all_16bit_value(self, value_r, value_g, value_b):
+    def set_pixel_all_16bit_value(
+        self, value_r: int, value_g: int, value_b: int
+    ) -> None:
         """
         Set the R, G, B values for all pixels.
 
         fast. without error checking.
 
         :param int value_r: 0..65535
         :param int value_g: 0..65535
         :param int value_b: 0..65535
         """
         for i in range(self.pixel_count):
             self.set_pixel_16bit_value(i, value_r, value_g, value_b)
 
-    def set_pixel_all(self, color):
+    def set_pixel_all(self, color: Tuple[float, float, float]) -> None:
         """
         Set the R, G, B values for all pixels.
 
-        :param tuple 3-tuple of R, G, B;  each int 0..65535 or float 0..1
+        :param tuple color: 3-tuple of R, G, B;  each int 0..65535 or float 0..1
         """
         for i in range(self.pixel_count):
             self.set_pixel(i, color)
 
-    def set_all_black(self):
+    def set_all_black(self) -> None:
         """Set all pixels to black."""
         for i in range(self.pixel_count):
             self.set_pixel_16bit_value(i, 0, 0, 0)
 
     # channel access
-    def set_channel(self, channel_index, value):
+    def set_channel(self, channel_index: int, value: int) -> None:
         """
         Set the value for the provided channel.
 
         :param int channel_index: 0..channel_count
         :param int value: 0..65535
         """
         if 0 <= channel_index < (self.channel_count):
@@ -858,81 +886,77 @@
             elif pixel_index_offset == 2:
                 channel_index -= 2
             # set value in buffer
             buffer_start = self._buffer_index_lookuptable[channel_index]
             struct.pack_into(">H", self._buffer, buffer_start, value)
         else:
             raise IndexError(
-                "channel_index {} out of range (0..{})".format(
-                    channel_index, self.channel_count
-                )
+                "channel_index {channel_index} out of range (0..{self.channel_count})"
             )
 
     # Define index and length properties to set and get each pixel as
     # atomic RGB tuples.  This provides a similar feel as using neopixels.
-    def __len__(self):
+    def __len__(self) -> int:
         """Retrieve TLC5975 the total number of Pixels available."""
         return self.pixel_count
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: int) -> Tuple[int, int, int]:
         """
         Retrieve the R, G, B values for the provided channel as a 3-tuple.
 
         Each value is a 16-bit number from 0-65535.
         """
         if 0 <= key < self.pixel_count:
             pixel_start = key * COLORS_PER_PIXEL
             return (
                 self._get_channel_16bit_value(pixel_start + 0),
                 self._get_channel_16bit_value(pixel_start + 1),
                 self._get_channel_16bit_value(pixel_start + 2),
             )
         # else:
-        raise IndexError("index {} out of range [0..{}]".format(key, self.pixel_count))
+        raise IndexError(f"index {key} out of range [0..{self.pixel_count}]")
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: int, value: Tuple[float, float, float]) -> None:
         """
         Set the R, G, B values for the pixel.
 
-        this funciton hase some advanced error checking.
+        this function has some advanced error checking.
         it is much slower than the other provided 'bare' variants..
         but therefor gives clues to what is going wrong.. ;-)
-        this shortcut is identicall to `set_pixel`
+        this shortcut is identical to `set_pixel`
 
         :param int key: 0..(pixel_count)
-        :param tuple 3-tuple of R, G, B;  each int 0..65535 or float 0..1
+        :param tuple value: 3-tuple of R, G, B;  each int 0..65535 or float 0..1
         """
         # for a more detailed version with all the debugging code and
         # comments look at set_pixel
         if 0 <= key < self.pixel_count:
             value = list(value)
             if len(value) != COLORS_PER_PIXEL:
                 raise IndexError(
-                    "length of value {} does not match COLORS_PER_PIXEL (= {})"
-                    "".format(len(value), COLORS_PER_PIXEL)
+                    f"length of value {len(value)} does not match COLORS_PER_PIXEL"
+                    " (= {COLORS_PER_PIXEL})"
                 )
             # _check_and_convert modifies value in place..
             self._check_and_convert(value)
             self.set_pixel_16bit_value(key, value[0], value[1], value[2])
         else:
-            raise IndexError(
-                "index {} out of range [0..{}]" "".format(key, self.pixel_count)
-            )
+            raise IndexError(f"index {key} out of range [0..{self.pixel_count}]")
 
     class _ChannelDirekt:
         # Internal decorator to simplify mapping.
 
-        def __init__(self, channel):
+        def __init__(self, channel) -> None:
             self._channel = channel
 
         def __get__(self, obj, obj_type):
             # Grab the 16-bit value at the offset for this channel.
             return obj._get_channel_16bit_value(self._channel)
 
-        def __set__(self, obj, value):
+        def __set__(self, obj, value) -> None:
             # Set the 16-bit value at the offset for this channel.
             assert 0 <= value <= 65535
             obj.set_channel(self._channel, value)
             # if obj.auto_show:
             #     obj._write()
 
     # Define explicit channels for first IC.
@@ -961,96 +985,96 @@
     This chip is designed to drive 4 RGB LEDs with 16-bit PWM per Color.
     The class has an interface compatible with the FancyLED library.
     and with this is similar to the NeoPixel and DotStar Interfaces.
 
     this TLC59711AutoShow is a subclass of TLC59711 that adds automatically
     sending changed data to the chips.
     this creates very slows responses on big changes.
-    It is mainly usefull if you only have a very small number of pixels.
+    It is mainly useful if you only have a very small number of pixels.
 
     :param ~busio.SPI spi: An instance of the SPI bus connected to the chip.
-        The clock and MOSI/outout must be set, the MISO/input is unused.
-        Maximal data clock frequence is:
+        The clock and MOSI/output must be set, the MISO/input is unused.
+        Maximal data clock frequency is:
         - TLC59711: 10MHz
         - TLC5971: 20MHz
-    :param bool pixel_count: Number of RGB-LEDs (=Pixels) that are connected.
+    :param int pixel_count: Number of RGB-LEDs (=Pixels) that are connected.
     """
 
-    def __init__(self, spi, pixel_count=4):
+    def __init__(self, spi: SPI, pixel_count: int = 4) -> None:
         """Init."""
         super().__init__(spi, pixel_count=pixel_count)
 
     ##########################################
 
-    def set_pixel(self, pixel_index, value):
+    def set_pixel(self, pixel_index: int, value: Tuple[float, float, float]) -> None:
         """
         Set the R, G, B values for the pixel.
 
-        this funciton hase some advanced error checking.
+        this function hase some advanced error checking.
         it is much slower than the other provided 'bare' variants..
         but therefor gives clues to what is going wrong.. ;-)
 
         :param int pixel_index: 0..(pixel_count)
         :param tuple value: 3-tuple of R, G, B;
             each int 0..65535 or float 0..1
         """
         super().set_pixel(pixel_index, value)
         self._write()
 
-    def set_pixel_all(self, color):
+    def set_pixel_all(self, color: Tuple[float, float, float]) -> None:
         """
         Set the R, G, B values for all pixels.
 
-        :param tuple 3-tuple of R, G, B;  each int 0..65535 or float 0..1
+        :param tuple color: 3-tuple of R, G, B;  each int 0..65535 or float 0..1
         """
         super().set_pixel_all(color)
         self._write()
 
-    def set_all_black(self):
+    def set_all_black(self) -> None:
         """Set all pixels to black."""
         super().set_all_black()
         self._write()
 
     # channel access
-    def set_channel(self, channel_index, value):
+    def set_channel(self, channel_index: int, value: int) -> None:
         """
         Set the value for the provided channel.
 
         :param int channel_index: 0..channel_count
         :param int value: 0..65535
         """
         super().set_channel(channel_index, value)
         self._write()
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: int, value: Tuple[float, float, float]) -> None:
         """
         Set the R, G, B values for the pixel.
 
-        this funciton hase some advanced error checking.
+        this function hase some advanced error checking.
         it is much slower than the other provided 'bare' variants..
         but therefor gives clues to what is going wrong.. ;-)
-        this shortcut is identicall to `set_pixel`
+        this shortcut is identical to `set_pixel`
 
         :param int key: 0..(pixel_count)
         :param tuple 3-tuple of R, G, B;  each int 0..65535 or float 0..1
         """
         super().__setitem__(key, value)
         self._write()
 
     class _ChannelDirektAutoShow:
         # Internal decorator to simplify mapping.
 
-        def __init__(self, channel):
+        def __init__(self, channel) -> None:
             self._channel = channel
 
         def __get__(self, obj, obj_type):
             # Grab the 16-bit value at the offset for this channel.
             return obj._get_channel_16bit_value(self._channel)
 
-        def __set__(self, obj, value):
+        def __set__(self, obj, value) -> None:
             # Set the 16-bit value at the offset for this channel.
             assert 0 <= value <= 65535
             obj.set_channel(self._channel, value)
             obj._write()
 
     # Define explicit channels for first IC.
     # → this is only for api backwards compliance.
```

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-tlc59711-2.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/docs/conf.py` & `adafruit-circuitpython-tlc59711-2.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/docs/examples.rst` & `adafruit-circuitpython-tlc59711-2.0.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/docs/index.rst` & `adafruit-circuitpython-tlc59711-2.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_dev.py` & `adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_dev.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_fancyled.py` & `adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_fancyled.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_fastset.py` & `adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_fastset.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_simpletest.py` & `adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_singlechip_autoshow.py` & `adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_singlechip_autoshow.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/examples/tlc59711_test_bcdata.py` & `adafruit-circuitpython-tlc59711-2.0.9/examples/tlc59711_test_bcdata.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc59711-2.0.8/pyproject.toml` & `adafruit-circuitpython-tlc59711-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-tlc59711"
 description = "CircuitPython library for TLC59711 16-bit 12 channel LED PWM driver."
-version = "2.0.8"
+version = "2.0.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_TLC59711"}
 keywords = [
     "adafruit",
```

