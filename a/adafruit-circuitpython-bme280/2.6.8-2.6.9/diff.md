# Comparing `tmp/adafruit-circuitpython-bme280-2.6.8.tar.gz` & `tmp/adafruit-circuitpython-bme280-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bme280-2.6.8.tar", last modified: Wed Dec 29 21:33:34 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-bme280-2.6.9.tar", last modified: Fri Feb  4 20:41:29 2022, max compression
```

## Comparing `adafruit-circuitpython-bme280-2.6.8.tar` & `adafruit-circuitpython-bme280-2.6.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:33:34.494520 adafruit-circuitpython-bme280-2.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:33:34.490520 adafruit-circuitpython-bme280-2.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:33:34.490520 adafruit-circuitpython-bme280-2.6.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:33:34.490520 adafruit-circuitpython-bme280-2.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      221 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:33:34.490520 adafruit-circuitpython-bme280-2.6.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5338 2021-12-29 21:33:34.494520 adafruit-circuitpython-bme280-2.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4494 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:33:34.490520 adafruit-circuitpython-bme280-2.6.8/adafruit_bme280/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/adafruit_bme280/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12881 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/adafruit_bme280/advanced.py
--rw-r--r--   0 runner    (1001) docker     (121)    15571 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/adafruit_bme280/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:33:34.490520 adafruit-circuitpython-bme280-2.6.8/adafruit_circuitpython_bme280.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5338 2021-12-29 21:33:34.000000 adafruit-circuitpython-bme280-2.6.8/adafruit_circuitpython_bme280.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2021-12-29 21:33:34.000000 adafruit-circuitpython-bme280-2.6.8/adafruit_circuitpython_bme280.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-29 21:33:34.000000 adafruit-circuitpython-bme280-2.6.8/adafruit_circuitpython_bme280.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-12-29 21:33:34.000000 adafruit-circuitpython-bme280-2.6.8/adafruit_circuitpython_bme280.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-12-29 21:33:34.000000 adafruit-circuitpython-bme280-2.6.8/adafruit_circuitpython_bme280.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:33:34.490520 adafruit-circuitpython-bme280-2.6.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:33:34.494520 adafruit-circuitpython-bme280-2.6.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5273 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:33:34.494520 adafruit-circuitpython-bme280-2.6.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/examples/bme280_normal_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/examples/bme280_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/examples/bme280_simpletest_pico.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-29 21:33:34.494520 adafruit-circuitpython-bme280-2.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2021-12-29 21:33:22.000000 adafruit-circuitpython-bme280-2.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:41:29.602547 adafruit-circuitpython-bme280-2.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:41:29.598546 adafruit-circuitpython-bme280-2.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:41:29.602547 adafruit-circuitpython-bme280-2.6.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:41:29.602547 adafruit-circuitpython-bme280-2.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:41:29.602547 adafruit-circuitpython-bme280-2.6.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5226 2022-02-04 20:41:29.602547 adafruit-circuitpython-bme280-2.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4482 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:41:29.602547 adafruit-circuitpython-bme280-2.6.9/adafruit_bme280/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/adafruit_bme280/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12881 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/adafruit_bme280/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15571 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/adafruit_bme280/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:41:29.602547 adafruit-circuitpython-bme280-2.6.9/adafruit_circuitpython_bme280.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5226 2022-02-04 20:41:29.000000 adafruit-circuitpython-bme280-2.6.9/adafruit_circuitpython_bme280.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-02-04 20:41:29.000000 adafruit-circuitpython-bme280-2.6.9/adafruit_circuitpython_bme280.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:41:29.000000 adafruit-circuitpython-bme280-2.6.9/adafruit_circuitpython_bme280.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-04 20:41:29.000000 adafruit-circuitpython-bme280-2.6.9/adafruit_circuitpython_bme280.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-04 20:41:29.000000 adafruit-circuitpython-bme280-2.6.9/adafruit_circuitpython_bme280.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:41:29.602547 adafruit-circuitpython-bme280-2.6.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:41:29.602547 adafruit-circuitpython-bme280-2.6.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5259 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:41:29.602547 adafruit-circuitpython-bme280-2.6.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/examples/bme280_normal_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)      877 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/examples/bme280_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      931 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/examples/bme280_simpletest_pico.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:41:29.602547 adafruit-circuitpython-bme280-2.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-02-04 20:41:17.000000 adafruit-circuitpython-bme280-2.6.9/setup.py
```

### Comparing `adafruit-circuitpython-bme280-2.6.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bme280-2.6.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

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

### Comparing `adafruit-circuitpython-bme280-2.6.8/.github/workflows/build.yml` & `adafruit-circuitpython-bme280-2.6.9/.github/workflows/build.yml`

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

### Comparing `adafruit-circuitpython-bme280-2.6.8/.github/workflows/release.yml` & `adafruit-circuitpython-bme280-2.6.9/.github/workflows/release.yml`

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

### Comparing `adafruit-circuitpython-bme280-2.6.8/.pre-commit-config.yaml` & `adafruit-circuitpython-bme280-2.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/.pylintrc` & `adafruit-circuitpython-bme280-2.6.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bme280-2.6.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/LICENSE` & `adafruit-circuitpython-bme280-2.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bme280-2.6.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/LICENSES/MIT.txt` & `adafruit-circuitpython-bme280-2.6.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bme280-2.6.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/PKG-INFO` & `adafruit-circuitpython-bme280-2.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bme280
-Version: 2.6.8
+Version: 2.6.9
 Summary: CircuitPython library for the Bosch BME280 temperature/humidity/pressure sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BME280
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit bme280 sensor hardware micropython circuitpython
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bme280/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/bme280/en/latest/
+    :target: https://docs.circuitpython.org/projects/bme280/en/latest/
     :alt: Documentation Status
 
 .. image :: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BME280/workflows/Build%20CI/badge.svg
@@ -124,15 +122,15 @@
         print("Pressure: %0.1f hPa" % bme280.pressure)
         print("Altitude = %0.2f meters" % bme280.altitude)
         time.sleep(2)
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/bme280/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bme280/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BME280/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-bme280-2.6.8/README.rst` & `adafruit-circuitpython-bme280-2.6.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bme280/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/bme280/en/latest/
+    :target: https://docs.circuitpython.org/projects/bme280/en/latest/
     :alt: Documentation Status
 
 .. image :: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BME280/workflows/Build%20CI/badge.svg
@@ -103,15 +103,15 @@
         print("Pressure: %0.1f hPa" % bme280.pressure)
         print("Altitude = %0.2f meters" % bme280.altitude)
         time.sleep(2)
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/bme280/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bme280/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BME280/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-bme280-2.6.8/adafruit_bme280/advanced.py` & `adafruit-circuitpython-bme280-2.6.9/adafruit_bme280/advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/adafruit_bme280/basic.py` & `adafruit-circuitpython-bme280-2.6.9/adafruit_bme280/basic.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/adafruit_circuitpython_bme280.egg-info/PKG-INFO` & `adafruit-circuitpython-bme280-2.6.9/adafruit_circuitpython_bme280.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bme280
-Version: 2.6.8
+Version: 2.6.9
 Summary: CircuitPython library for the Bosch BME280 temperature/humidity/pressure sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BME280
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit bme280 sensor hardware micropython circuitpython
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bme280/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/bme280/en/latest/
+    :target: https://docs.circuitpython.org/projects/bme280/en/latest/
     :alt: Documentation Status
 
 .. image :: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BME280/workflows/Build%20CI/badge.svg
@@ -124,15 +122,15 @@
         print("Pressure: %0.1f hPa" % bme280.pressure)
         print("Altitude = %0.2f meters" % bme280.altitude)
         time.sleep(2)
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/bme280/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bme280/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BME280/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-bme280-2.6.8/adafruit_circuitpython_bme280.egg-info/SOURCES.txt` & `adafruit-circuitpython-bme280-2.6.9/adafruit_circuitpython_bme280.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/docs/_static/favicon.ico` & `adafruit-circuitpython-bme280-2.6.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/docs/conf.py` & `adafruit-circuitpython-bme280-2.6.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
 ]
 
 # API docs fix
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

### Comparing `adafruit-circuitpython-bme280-2.6.8/docs/examples.rst` & `adafruit-circuitpython-bme280-2.6.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/docs/index.rst` & `adafruit-circuitpython-bme280-2.6.9/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     Adafruit BME280 I2C or SPI Temperature Humidity Pressure Sensor  <https://www.adafruit.com/product/2652>
 
 .. toctree::
     :caption: Other Links
 
     Download <https://github.com/adafruit/Adafruit_CircuitPython_BME280/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-bme280-2.6.8/examples/bme280_normal_mode.py` & `adafruit-circuitpython-bme280-2.6.9/examples/bme280_normal_mode.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/examples/bme280_simpletest.py` & `adafruit-circuitpython-bme280-2.6.9/examples/bme280_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/examples/bme280_simpletest_pico.py` & `adafruit-circuitpython-bme280-2.6.9/examples/bme280_simpletest_pico.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme280-2.6.8/setup.py` & `adafruit-circuitpython-bme280-2.6.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,16 +41,14 @@
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
     keywords="adafruit bme280 sensor hardware micropython circuitpython",
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     packages=["adafruit_bme280"],
 )
```

