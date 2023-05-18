# Comparing `tmp/adafruit-circuitpython-tlc5947-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-tlc5947-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tlc5947-1.3.8.tar", last modified: Thu Jun  9 18:34:27 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-tlc5947-1.3.9.tar", last modified: Tue Aug  9 19:56:23 2022, max compression
```

## Comparing `adafruit-circuitpython-tlc5947-1.3.8.tar` & `adafruit-circuitpython-tlc5947-1.3.9.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:34:27.803424 adafruit-circuitpython-tlc5947-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:34:27.791424 adafruit-circuitpython-tlc5947-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:34:27.795424 adafruit-circuitpython-tlc5947-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:34:27.799424 adafruit-circuitpython-tlc5947-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:34:27.799424 adafruit-circuitpython-tlc5947-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-06-09 18:34:27.803424 adafruit-circuitpython-tlc5947-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:34:27.799424 adafruit-circuitpython-tlc5947-1.3.8/adafruit_circuitpython_tlc5947.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-06-09 18:34:27.000000 adafruit-circuitpython-tlc5947-1.3.8/adafruit_circuitpython_tlc5947.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-06-09 18:34:27.000000 adafruit-circuitpython-tlc5947-1.3.8/adafruit_circuitpython_tlc5947.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:34:27.000000 adafruit-circuitpython-tlc5947-1.3.8/adafruit_circuitpython_tlc5947.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-09 18:34:27.000000 adafruit-circuitpython-tlc5947-1.3.8/adafruit_circuitpython_tlc5947.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11502 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/adafruit_tlc5947.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:34:27.803424 adafruit-circuitpython-tlc5947-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:34:27.803424 adafruit-circuitpython-tlc5947-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5350 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:34:27.803424 adafruit-circuitpython-tlc5947-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     4416 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/examples/tlc5947_chain.py
--rw-r--r--   0 runner    (1001) docker     (121)     2641 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/examples/tlc5947_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:34:27.803424 adafruit-circuitpython-tlc5947-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-06-09 18:34:13.000000 adafruit-circuitpython-tlc5947-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:56:23.443962 adafruit-circuitpython-tlc5947-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:56:23.439962 adafruit-circuitpython-tlc5947-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:56:23.439962 adafruit-circuitpython-tlc5947-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:56:23.439962 adafruit-circuitpython-tlc5947-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:56:23.439962 adafruit-circuitpython-tlc5947-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3386 2022-08-09 19:56:23.443962 adafruit-circuitpython-tlc5947-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2604 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:56:23.439962 adafruit-circuitpython-tlc5947-1.3.9/adafruit_circuitpython_tlc5947.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3386 2022-08-09 19:56:23.000000 adafruit-circuitpython-tlc5947-1.3.9/adafruit_circuitpython_tlc5947.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-08-09 19:56:23.000000 adafruit-circuitpython-tlc5947-1.3.9/adafruit_circuitpython_tlc5947.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:56:23.000000 adafruit-circuitpython-tlc5947-1.3.9/adafruit_circuitpython_tlc5947.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-09 19:56:23.000000 adafruit-circuitpython-tlc5947-1.3.9/adafruit_circuitpython_tlc5947.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-09 19:56:23.000000 adafruit-circuitpython-tlc5947-1.3.9/adafruit_circuitpython_tlc5947.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11495 2022-08-09 19:56:13.000000 adafruit-circuitpython-tlc5947-1.3.9/adafruit_tlc5947.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:56:23.443962 adafruit-circuitpython-tlc5947-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:56:23.443962 adafruit-circuitpython-tlc5947-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5350 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:56:23.443962 adafruit-circuitpython-tlc5947-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     4416 2022-08-09 19:56:13.000000 adafruit-circuitpython-tlc5947-1.3.9/examples/tlc5947_chain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2641 2022-08-09 19:56:13.000000 adafruit-circuitpython-tlc5947-1.3.9/examples/tlc5947_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-08-09 19:56:13.000000 adafruit-circuitpython-tlc5947-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-09 19:55:52.000000 adafruit-circuitpython-tlc5947-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:56:23.443962 adafruit-circuitpython-tlc5947-1.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tlc5947-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-tlc5947-1.3.9/.github/workflows/build.yml`

 * *Files 16% similar despite different names*

```diff
@@ -43,33 +43,35 @@
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
     - name: Archive bundles
       uses: actions/upload-artifact@v2
       with:
         name: bundles
         path: ${{ github.workspace }}/bundles/
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

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/.gitignore` & `adafruit-circuitpython-tlc5947-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-tlc5947-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/.pylintrc` & `adafruit-circuitpython-tlc5947-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tlc5947-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/LICENSE` & `adafruit-circuitpython-tlc5947-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tlc5947-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-tlc5947-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tlc5947-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/PKG-INFO` & `adafruit-circuitpython-tlc5947-1.3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tlc5947
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for TLC5947 12-bit 24 channel LED PWM driver.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TLC5947
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit tlc5947 12-bit 24-channel led pwm hardware micropython circuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TLC5947
+Keywords: adafruit,tlc5947,12-bit,24-channel,led,pwm,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-tlc5947/badge/?version=latest
@@ -29,14 +28,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_TLC5947/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_TLC5947/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython module for the TLC5947 12-bit 24 channel LED PWM driver.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -62,16 +65,16 @@
     sudo pip3 install adafruit-circuitpython-tlc5947
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-tlc5947
 
 Usage Example
 =============
 
 | See examples/tlc5947_simpletest.py for a demo of the usage.
 | See examples/tlc5947_chain.py for a demo of chained driver usage.
@@ -85,9 +88,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_TLC5947/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/README.rst` & `adafruit-circuitpython-tlc5947-1.3.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_TLC5947/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_TLC5947/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython module for the TLC5947 12-bit 24 channel LED PWM driver.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -43,16 +47,16 @@
     sudo pip3 install adafruit-circuitpython-tlc5947
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-tlc5947
 
 Usage Example
 =============
 
 | See examples/tlc5947_simpletest.py for a demo of the usage.
 | See examples/tlc5947_chain.py for a demo of chained driver usage.
```

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/adafruit_circuitpython_tlc5947.egg-info/PKG-INFO` & `adafruit-circuitpython-tlc5947-1.3.9/adafruit_circuitpython_tlc5947.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tlc5947
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for TLC5947 12-bit 24 channel LED PWM driver.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TLC5947
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit tlc5947 12-bit 24-channel led pwm hardware micropython circuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TLC5947
+Keywords: adafruit,tlc5947,12-bit,24-channel,led,pwm,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-tlc5947/badge/?version=latest
@@ -29,14 +28,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_TLC5947/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_TLC5947/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython module for the TLC5947 12-bit 24 channel LED PWM driver.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -62,16 +65,16 @@
     sudo pip3 install adafruit-circuitpython-tlc5947
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-tlc5947
 
 Usage Example
 =============
 
 | See examples/tlc5947_simpletest.py for a demo of the usage.
 | See examples/tlc5947_chain.py for a demo of chained driver usage.
@@ -85,9 +88,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_TLC5947/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/adafruit_circuitpython_tlc5947.egg-info/SOURCES.txt` & `adafruit-circuitpython-tlc5947-1.3.9/adafruit_circuitpython_tlc5947.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_tlc5947.py
+optional_requirements.txt
+pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_tlc5947.egg-info/PKG-INFO
 adafruit_circuitpython_tlc5947.egg-info/SOURCES.txt
 adafruit_circuitpython_tlc5947.egg-info/dependency_links.txt
+adafruit_circuitpython_tlc5947.egg-info/requires.txt
 adafruit_circuitpython_tlc5947.egg-info/top_level.txt
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
```

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/adafruit_tlc5947.py` & `adafruit-circuitpython-tlc5947-1.3.9/adafruit_tlc5947.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   <https://www.adafruit.com/product/1429>`_ (Product ID: 1429)
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the ESP8622 and M0-based boards:
   https://github.com/adafruit/circuitpython/releases
 """
-__version__ = "0.0.0-auto.0"
+__version__ = "1.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_TLC5947.git"
 
 
 # Globally disable protected access.  Ppylint can't figure out the
 # context for using internal decorate classes below.  In these cases protectected
 # access is by design for the internal class.
 # pylint: disable=protected-access
```

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-tlc5947-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/docs/conf.py` & `adafruit-circuitpython-tlc5947-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/docs/index.rst` & `adafruit-circuitpython-tlc5947-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/examples/tlc5947_chain.py` & `adafruit-circuitpython-tlc5947-1.3.9/examples/tlc5947_chain.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlc5947-1.3.8/examples/tlc5947_simpletest.py` & `adafruit-circuitpython-tlc5947-1.3.9/examples/tlc5947_simpletest.py`

 * *Files identical despite different names*

