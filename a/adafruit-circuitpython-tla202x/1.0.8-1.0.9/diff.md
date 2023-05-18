# Comparing `tmp/adafruit-circuitpython-tla202x-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-tla202x-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tla202x-1.0.8.tar", last modified: Thu Jun  9 18:29:35 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-tla202x-1.0.9.tar", last modified: Tue Aug  9 19:51:46 2022, max compression
```

## Comparing `adafruit-circuitpython-tla202x-1.0.8.tar` & `adafruit-circuitpython-tla202x-1.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:35.385614 adafruit-circuitpython-tla202x-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:35.381614 adafruit-circuitpython-tla202x-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:35.381614 adafruit-circuitpython-tla202x-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:35.381614 adafruit-circuitpython-tla202x-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:35.381614 adafruit-circuitpython-tla202x-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-06-09 18:29:35.385614 adafruit-circuitpython-tla202x-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2863 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:35.381614 adafruit-circuitpython-tla202x-1.0.8/adafruit_circuitpython_tla202x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-06-09 18:29:35.000000 adafruit-circuitpython-tla202x-1.0.8/adafruit_circuitpython_tla202x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-09 18:29:35.000000 adafruit-circuitpython-tla202x-1.0.8/adafruit_circuitpython_tla202x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:29:35.000000 adafruit-circuitpython-tla202x-1.0.8/adafruit_circuitpython_tla202x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-09 18:29:35.000000 adafruit-circuitpython-tla202x-1.0.8/adafruit_circuitpython_tla202x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-09 18:29:35.000000 adafruit-circuitpython-tla202x-1.0.8/adafruit_circuitpython_tla202x.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:35.381614 adafruit-circuitpython-tla202x-1.0.8/adafruit_tla202x/
--rw-r--r--   0 runner    (1001) docker     (121)    13170 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/adafruit_tla202x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2965 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/adafruit_tla202x/analog_in.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/adafruit_tla202x/tla2024.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:35.381614 adafruit-circuitpython-tla202x-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:35.381614 adafruit-circuitpython-tla202x-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5767 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:29:35.381614 adafruit-circuitpython-tla202x-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/examples/tla202x_analog_in.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/examples/tla202x_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/examples/tla202x_mux_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/examples/tla202x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:29:35.385614 adafruit-circuitpython-tla202x-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-06-09 18:29:22.000000 adafruit-circuitpython-tla202x-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:51:46.160348 adafruit-circuitpython-tla202x-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:51:46.156348 adafruit-circuitpython-tla202x-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:51:46.156348 adafruit-circuitpython-tla202x-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:51:46.156348 adafruit-circuitpython-tla202x-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:51:46.156348 adafruit-circuitpython-tla202x-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3645 2022-08-09 19:51:46.160348 adafruit-circuitpython-tla202x-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:51:46.156348 adafruit-circuitpython-tla202x-1.0.9/adafruit_circuitpython_tla202x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3645 2022-08-09 19:51:46.000000 adafruit-circuitpython-tla202x-1.0.9/adafruit_circuitpython_tla202x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-08-09 19:51:46.000000 adafruit-circuitpython-tla202x-1.0.9/adafruit_circuitpython_tla202x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:51:46.000000 adafruit-circuitpython-tla202x-1.0.9/adafruit_circuitpython_tla202x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-09 19:51:46.000000 adafruit-circuitpython-tla202x-1.0.9/adafruit_circuitpython_tla202x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-09 19:51:46.000000 adafruit-circuitpython-tla202x-1.0.9/adafruit_circuitpython_tla202x.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:51:46.156348 adafruit-circuitpython-tla202x-1.0.9/adafruit_tla202x/
+-rw-r--r--   0 runner    (1001) docker     (121)    13163 2022-08-09 19:51:38.000000 adafruit-circuitpython-tla202x-1.0.9/adafruit_tla202x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2965 2022-08-09 19:51:38.000000 adafruit-circuitpython-tla202x-1.0.9/adafruit_tla202x/analog_in.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-08-09 19:51:38.000000 adafruit-circuitpython-tla202x-1.0.9/adafruit_tla202x/tla2024.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:51:46.160348 adafruit-circuitpython-tla202x-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:51:46.160348 adafruit-circuitpython-tla202x-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5767 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:51:46.160348 adafruit-circuitpython-tla202x-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-08-09 19:51:38.000000 adafruit-circuitpython-tla202x-1.0.9/examples/tla202x_analog_in.py
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-08-09 19:51:38.000000 adafruit-circuitpython-tla202x-1.0.9/examples/tla202x_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-08-09 19:51:38.000000 adafruit-circuitpython-tla202x-1.0.9/examples/tla202x_mux_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2022-08-09 19:51:38.000000 adafruit-circuitpython-tla202x-1.0.9/examples/tla202x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-08-09 19:51:38.000000 adafruit-circuitpython-tla202x-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-09 19:51:28.000000 adafruit-circuitpython-tla202x-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:51:46.160348 adafruit-circuitpython-tla202x-1.0.9/setup.cfg
```

### Comparing `adafruit-circuitpython-tla202x-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tla202x-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-tla202x-1.0.9/.github/workflows/build.yml`

 * *Files 20% similar despite different names*

```diff
@@ -43,28 +43,35 @@
       run: |
         source actions-ci/install.sh
     - name: Pip install Sphinx, pre-commit
       run: |
         pip install --force-reinstall Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
+    - name: Setup problem matchers
+      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
+    - name: Archive bundles
+      uses: actions/upload-artifact@v2
+      with:
+        name: bundles
+        path: ${{ github.workspace }}/bundles/
     - name: Build docs
       working-directory: docs
       run: sphinx-build -E -W -b html . _build/html
-    - name: Check For setup.py
+    - name: Check For pyproject.toml
       id: need-pypi
       run: |
-        echo ::set-output name=setup-py::$( find . -wholename './setup.py' )
+        echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
-      if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
+      if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
-        pip install --upgrade setuptools wheel twine readme_renderer testresources
-        python setup.py sdist
-        python setup.py bdist_wheel --universal
+        pip install --upgrade build twine
+        for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
+            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+        done;
+        python -m build
         twine check dist/*
-    - name: Setup problem matchers
-      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
```

### Comparing `adafruit-circuitpython-tla202x-1.0.8/.gitignore` & `adafruit-circuitpython-tla202x-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-tla202x-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/.pylintrc` & `adafruit-circuitpython-tla202x-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tla202x-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/LICENSE` & `adafruit-circuitpython-tla202x-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tla202x-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-tla202x-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tla202x-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/PKG-INFO` & `adafruit-circuitpython-tla202x-1.0.9/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: adafruit-circuitpython-tla202x
-Version: 1.0.8
-Summary: Library for the TI TLA202x 12-bit ADCs
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TLA202x
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
-License: MIT
-Keywords: adafruit blinka circuitpython micropython tla202x TLA2021 TLA2022 TLA2024 ADC Delta-Sigma Analog Voltage
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: System :: Hardware
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-tla202x/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/tla202x/en/latest/
     :alt: Documentation Status
 
@@ -67,16 +48,16 @@
     sudo pip3 install adafruit-circuitpython-tla202x
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-tla202x
 
 Usage Example
 =============
 
 .. code-block:: python3
 
@@ -101,9 +82,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_TLA202x/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-tla202x-1.0.8/adafruit_circuitpython_tla202x.egg-info/SOURCES.txt` & `adafruit-circuitpython-tla202x-1.0.9/adafruit_circuitpython_tla202x.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
+optional_requirements.txt
 pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
```

### Comparing `adafruit-circuitpython-tla202x-1.0.8/adafruit_tla202x/__init__.py` & `adafruit-circuitpython-tla202x-1.0.9/adafruit_tla202x/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 try:
     from typing import Tuple, Union, Optional
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_TLA202x.git"
 
 _TLA_DEFAULT_ADDRESS = const(0x48)
 _DATA_REG = const(0x00)
 _CONFIG_REG = const(0x01)
```

### Comparing `adafruit-circuitpython-tla202x-1.0.8/adafruit_tla202x/analog_in.py` & `adafruit-circuitpython-tla202x-1.0.9/adafruit_tla202x/analog_in.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/adafruit_tla202x/tla2024.py` & `adafruit-circuitpython-tla202x-1.0.9/adafruit_tla202x/tla2024.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-tla202x-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/docs/conf.py` & `adafruit-circuitpython-tla202x-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/docs/index.rst` & `adafruit-circuitpython-tla202x-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/examples/tla202x_analog_in.py` & `adafruit-circuitpython-tla202x-1.0.9/examples/tla202x_analog_in.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tla202x-1.0.8/examples/tla202x_mux_test.py` & `adafruit-circuitpython-tla202x-1.0.9/examples/tla202x_mux_test.py`

 * *Files identical despite different names*

