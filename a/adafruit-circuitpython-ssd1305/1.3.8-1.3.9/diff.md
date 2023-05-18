# Comparing `tmp/adafruit-circuitpython-ssd1305-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-ssd1305-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1305-1.3.8.tar", last modified: Mon Nov 15 19:11:11 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1305-1.3.9.tar", last modified: Fri Feb  4 20:25:00 2022, max compression
```

## Comparing `adafruit-circuitpython-ssd1305-1.3.8.tar` & `adafruit-circuitpython-ssd1305-1.3.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.506473 adafruit-circuitpython-ssd1305-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.498473 adafruit-circuitpython-ssd1305-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.502473 adafruit-circuitpython-ssd1305-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.502473 adafruit-circuitpython-ssd1305-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      197 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.502473 adafruit-circuitpython-ssd1305-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4173 2021-11-15 19:11:11.506473 adafruit-circuitpython-ssd1305-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3350 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.502473 adafruit-circuitpython-ssd1305-1.3.8/adafruit_circuitpython_ssd1305.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4173 2021-11-15 19:11:11.000000 adafruit-circuitpython-ssd1305-1.3.8/adafruit_circuitpython_ssd1305.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      952 2021-11-15 19:11:11.000000 adafruit-circuitpython-ssd1305-1.3.8/adafruit_circuitpython_ssd1305.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 19:11:11.000000 adafruit-circuitpython-ssd1305-1.3.8/adafruit_circuitpython_ssd1305.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-11-15 19:11:11.000000 adafruit-circuitpython-ssd1305-1.3.8/adafruit_circuitpython_ssd1305.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-11-15 19:11:11.000000 adafruit-circuitpython-ssd1305-1.3.8/adafruit_circuitpython_ssd1305.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9987 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/adafruit_ssd1305.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.506473 adafruit-circuitpython-ssd1305-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.506473 adafruit-circuitpython-ssd1305-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5621 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      900 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.506473 adafruit-circuitpython-ssd1305-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1857 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/examples/ssd1305_pillow_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/examples/ssd1305_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/examples/ssd1305_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 19:11:11.506473 adafruit-circuitpython-ssd1305-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2021-11-15 19:10:55.000000 adafruit-circuitpython-ssd1305-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:25:00.597917 adafruit-circuitpython-ssd1305-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:25:00.589917 adafruit-circuitpython-ssd1305-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:25:00.593917 adafruit-circuitpython-ssd1305-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:25:00.593917 adafruit-circuitpython-ssd1305-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:25:00.593917 adafruit-circuitpython-ssd1305-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4061 2022-02-04 20:25:00.597917 adafruit-circuitpython-ssd1305-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3338 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:25:00.593917 adafruit-circuitpython-ssd1305-1.3.9/adafruit_circuitpython_ssd1305.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4061 2022-02-04 20:25:00.000000 adafruit-circuitpython-ssd1305-1.3.9/adafruit_circuitpython_ssd1305.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-02-04 20:25:00.000000 adafruit-circuitpython-ssd1305-1.3.9/adafruit_circuitpython_ssd1305.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:25:00.000000 adafruit-circuitpython-ssd1305-1.3.9/adafruit_circuitpython_ssd1305.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-04 20:25:00.000000 adafruit-circuitpython-ssd1305-1.3.9/adafruit_circuitpython_ssd1305.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-04 20:25:00.000000 adafruit-circuitpython-ssd1305-1.3.9/adafruit_circuitpython_ssd1305.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9987 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/adafruit_ssd1305.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:25:00.597917 adafruit-circuitpython-ssd1305-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:25:00.597917 adafruit-circuitpython-ssd1305-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5607 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      894 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:25:00.597917 adafruit-circuitpython-ssd1305-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1857 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/examples/ssd1305_pillow_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/examples/ssd1305_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/examples/ssd1305_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:25:00.597917 adafruit-circuitpython-ssd1305-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1865 2022-02-04 20:24:47.000000 adafruit-circuitpython-ssd1305-1.3.9/setup.py
```

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1305-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2021 Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 Thank you for contributing! Before you submit a pull request, please read the following.
 
-Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://circuitpython.readthedocs.io/en/latest/docs/design_guide.html
+Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://docs.circuitpython.org/en/latest/docs/design_guide.html
 
 If your changes are to documentation, please verify that the documentation builds locally by following the steps found here: https://adafru.it/build-docs
 
 Before submitting the pull request, make sure you've run Pylint and Black locally on your code. You can do this manually or using pre-commit. Instructions are available here: https://adafru.it/check-your-code
 
 Please remove all of this text before submitting. Include an explanation or list of changes included in your PR, as well as, if applicable, a link to any related issues.
```

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-ssd1305-1.3.9/.github/workflows/build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.7
-      uses: actions/setup-python@v1
+    - name: Set up Python 3.x
+      uses: actions/setup-python@v2
       with:
-        python-version: 3.7
+        python-version: "3.x"
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v1
       with:
         submodules: true
```

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-ssd1305-1.3.9/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.6
-      uses: actions/setup-python@v1
+    - name: Set up Python 3.x
+      uses: actions/setup-python@v2
       with:
-        python-version: 3.6
+        python-version: "3.x"
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v1
       with:
         submodules: true
@@ -63,15 +63,15 @@
     - uses: actions/checkout@v1
     - name: Check For setup.py
       id: need-pypi
       run: |
         echo ::set-output name=setup-py::$( find . -wholename './setup.py' )
     - name: Set up Python
       if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v2
       with:
         python-version: '3.x'
     - name: Install dependencies
       if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
```

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1305-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/.pylintrc` & `adafruit-circuitpython-ssd1305-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1305-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/LICENSE` & `adafruit-circuitpython-ssd1305-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1305-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1305-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1305-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/PKG-INFO` & `adafruit-circuitpython-ssd1305-1.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1305
-Version: 1.3.8
+Version: 1.3.9
 Summary: Framebuf (non-displayio) driver for SSD1305 displays
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SSD1305
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ssd1305 framebuf rpi
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1305/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ssd1305/en/latest/
+    :target: https://docs.circuitpython.org/projects/ssd1305/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SSD1305/workflows/Build%20CI/badge.svg
@@ -106,15 +104,15 @@
     display.fill(0)
 
     display.show()
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ssd1305/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ssd1305/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_SSD1305/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/README.rst` & `adafruit-circuitpython-ssd1305-1.3.9/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1305/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ssd1305/en/latest/
+    :target: https://docs.circuitpython.org/projects/ssd1305/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SSD1305/workflows/Build%20CI/badge.svg
@@ -85,15 +85,15 @@
     display.fill(0)
 
     display.show()
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ssd1305/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ssd1305/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_SSD1305/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/adafruit_circuitpython_ssd1305.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1305-1.3.9/adafruit_circuitpython_ssd1305.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1305
-Version: 1.3.8
+Version: 1.3.9
 Summary: Framebuf (non-displayio) driver for SSD1305 displays
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SSD1305
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ssd1305 framebuf rpi
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1305/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ssd1305/en/latest/
+    :target: https://docs.circuitpython.org/projects/ssd1305/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SSD1305/workflows/Build%20CI/badge.svg
@@ -106,15 +104,15 @@
     display.fill(0)
 
     display.show()
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ssd1305/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ssd1305/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_SSD1305/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/adafruit_circuitpython_ssd1305.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1305-1.3.9/adafruit_circuitpython_ssd1305.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/adafruit_ssd1305.py` & `adafruit-circuitpython-ssd1305-1.3.9/adafruit_ssd1305.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1305-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/docs/conf.py` & `adafruit-circuitpython-ssd1305-1.3.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,20 @@
     "adafruit_bus_device",
     "adafruit_framebuf",
     "busio",
 ]
 
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3.4", None),
+    "python": ("https://docs.python.org/3", None),
     "BusDevice": (
-        "https://circuitpython.readthedocs.io/projects/busdevice/en/latest/",
+        "https://docs.circuitpython.org/projects/busdevice/en/latest/",
         None,
     ),
-    "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
+    "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 source_suffix = ".rst"
```

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/docs/index.rst` & `adafruit-circuitpython-ssd1305-1.3.9/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 .. toctree::
     :caption: Related Products
 
 .. toctree::
     :caption: Other Links
 
     Download <https://github.com/adafruit/Adafruit_CircuitPython_SSD1305/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/examples/ssd1305_pillow_demo.py` & `adafruit-circuitpython-ssd1305-1.3.9/examples/ssd1305_pillow_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/examples/ssd1305_simpletest.py` & `adafruit-circuitpython-ssd1305-1.3.9/examples/ssd1305_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/examples/ssd1305_stats.py` & `adafruit-circuitpython-ssd1305-1.3.9/examples/ssd1305_stats.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1305-1.3.8/setup.py` & `adafruit-circuitpython-ssd1305-1.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,16 +44,14 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "Topic :: System :: Hardware",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
     ],
     # What does your project relate to?
     keywords="adafruit blinka circuitpython micropython ssd1305 framebuf rpi",
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     py_modules=["adafruit_ssd1305"],
 )
```

