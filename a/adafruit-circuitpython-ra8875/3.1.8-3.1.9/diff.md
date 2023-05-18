# Comparing `tmp/adafruit-circuitpython-ra8875-3.1.8.tar.gz` & `tmp/adafruit-circuitpython-ra8875-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ra8875-3.1.8.tar", last modified: Mon Dec 27 22:38:25 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-ra8875-3.1.9.tar", last modified: Fri Feb  4 21:04:49 2022, max compression
```

## Comparing `adafruit-circuitpython-ra8875-3.1.8.tar` & `adafruit-circuitpython-ra8875-3.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 22:38:25.451149 adafruit-circuitpython-ra8875-3.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 22:38:25.447149 adafruit-circuitpython-ra8875-3.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 22:38:25.447149 adafruit-circuitpython-ra8875-3.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 22:38:25.451149 adafruit-circuitpython-ra8875-3.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 22:38:25.451149 adafruit-circuitpython-ra8875-3.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3778 2021-12-27 22:38:25.451149 adafruit-circuitpython-ra8875-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 22:38:25.451149 adafruit-circuitpython-ra8875-3.1.8/adafruit_circuitpython_ra8875.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3778 2021-12-27 22:38:25.000000 adafruit-circuitpython-ra8875-3.1.8/adafruit_circuitpython_ra8875.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2021-12-27 22:38:25.000000 adafruit-circuitpython-ra8875-3.1.8/adafruit_circuitpython_ra8875.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-27 22:38:25.000000 adafruit-circuitpython-ra8875-3.1.8/adafruit_circuitpython_ra8875.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-12-27 22:38:25.000000 adafruit-circuitpython-ra8875-3.1.8/adafruit_circuitpython_ra8875.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-12-27 22:38:25.000000 adafruit-circuitpython-ra8875-3.1.8/adafruit_circuitpython_ra8875.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 22:38:25.451149 adafruit-circuitpython-ra8875-3.1.8/adafruit_ra8875/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/adafruit_ra8875/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    32139 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/adafruit_ra8875/ra8875.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2333 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/adafruit_ra8875/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 22:38:25.451149 adafruit-circuitpython-ra8875-3.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 22:38:25.451149 adafruit-circuitpython-ra8875-3.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5571 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      319 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 22:38:25.451149 adafruit-circuitpython-ra8875-3.1.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)   150584 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/examples/ra8875_blinka.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/examples/ra8875_blinka.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     3205 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/examples/ra8875_bmptest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/examples/ra8875_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-27 22:38:25.451149 adafruit-circuitpython-ra8875-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2021-12-27 22:38:14.000000 adafruit-circuitpython-ra8875-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:49.227253 adafruit-circuitpython-ra8875-3.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:49.219252 adafruit-circuitpython-ra8875-3.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:49.223253 adafruit-circuitpython-ra8875-3.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:49.223253 adafruit-circuitpython-ra8875-3.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:49.223253 adafruit-circuitpython-ra8875-3.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-02-04 21:04:49.227253 adafruit-circuitpython-ra8875-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:49.223253 adafruit-circuitpython-ra8875-3.1.9/adafruit_circuitpython_ra8875.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-02-04 21:04:49.000000 adafruit-circuitpython-ra8875-3.1.9/adafruit_circuitpython_ra8875.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-02-04 21:04:49.000000 adafruit-circuitpython-ra8875-3.1.9/adafruit_circuitpython_ra8875.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 21:04:49.000000 adafruit-circuitpython-ra8875-3.1.9/adafruit_circuitpython_ra8875.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-04 21:04:49.000000 adafruit-circuitpython-ra8875-3.1.9/adafruit_circuitpython_ra8875.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-04 21:04:49.000000 adafruit-circuitpython-ra8875-3.1.9/adafruit_circuitpython_ra8875.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:49.223253 adafruit-circuitpython-ra8875-3.1.9/adafruit_ra8875/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/adafruit_ra8875/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    32139 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/adafruit_ra8875/ra8875.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2333 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/adafruit_ra8875/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:49.227253 adafruit-circuitpython-ra8875-3.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:49.227253 adafruit-circuitpython-ra8875-3.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5557 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:49.227253 adafruit-circuitpython-ra8875-3.1.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (121)   150584 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/examples/ra8875_blinka.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/examples/ra8875_blinka.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3205 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/examples/ra8875_bmptest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/examples/ra8875_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 21:04:49.227253 adafruit-circuitpython-ra8875-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-02-04 21:04:38.000000 adafruit-circuitpython-ra8875-3.1.9/setup.py
```

### Comparing `adafruit-circuitpython-ra8875-3.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ra8875-3.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

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

### Comparing `adafruit-circuitpython-ra8875-3.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-ra8875-3.1.9/.github/workflows/build.yml`

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

### Comparing `adafruit-circuitpython-ra8875-3.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-ra8875-3.1.9/.github/workflows/release.yml`

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

### Comparing `adafruit-circuitpython-ra8875-3.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ra8875-3.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/.pylintrc` & `adafruit-circuitpython-ra8875-3.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ra8875-3.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/LICENSE` & `adafruit-circuitpython-ra8875-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ra8875-3.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ra8875-3.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ra8875-3.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/PKG-INFO` & `adafruit-circuitpython-ra8875-3.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ra8875
-Version: 3.1.8
+Version: 3.1.9
 Summary: CircuitPython driver for TFT Touch screens based on RA8875.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_RA8875
 Author: Melissa LeBlanc-Williams & Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit ra8875 display driver tft touch screen hardware micropython circuitpython
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ra8875/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ra8875/en/latest/
+    :target: https://docs.circuitpython.org/projects/ra8875/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_RA8875/workflows/Build%20CI/badge.svg
@@ -81,15 +79,15 @@
 
 See examples/ra8875_simpletest.py and examples/ra8875_bmptest.py for examples of the module's usage. When
 running the bmptest, be sure to upload the blinka.bmp image to the root folder as well.
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ra8875/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ra8875/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_RA8875/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ra8875-3.1.8/README.rst` & `adafruit-circuitpython-ra8875-3.1.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ra8875/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ra8875/en/latest/
+    :target: https://docs.circuitpython.org/projects/ra8875/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_RA8875/workflows/Build%20CI/badge.svg
@@ -60,15 +60,15 @@
 
 See examples/ra8875_simpletest.py and examples/ra8875_bmptest.py for examples of the module's usage. When
 running the bmptest, be sure to upload the blinka.bmp image to the root folder as well.
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ra8875/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ra8875/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_RA8875/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ra8875-3.1.8/adafruit_circuitpython_ra8875.egg-info/PKG-INFO` & `adafruit-circuitpython-ra8875-3.1.9/adafruit_circuitpython_ra8875.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ra8875
-Version: 3.1.8
+Version: 3.1.9
 Summary: CircuitPython driver for TFT Touch screens based on RA8875.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_RA8875
 Author: Melissa LeBlanc-Williams & Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit ra8875 display driver tft touch screen hardware micropython circuitpython
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ra8875/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ra8875/en/latest/
+    :target: https://docs.circuitpython.org/projects/ra8875/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_RA8875/workflows/Build%20CI/badge.svg
@@ -81,15 +79,15 @@
 
 See examples/ra8875_simpletest.py and examples/ra8875_bmptest.py for examples of the module's usage. When
 running the bmptest, be sure to upload the blinka.bmp image to the root folder as well.
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ra8875/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ra8875/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_RA8875/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ra8875-3.1.8/adafruit_circuitpython_ra8875.egg-info/SOURCES.txt` & `adafruit-circuitpython-ra8875-3.1.9/adafruit_circuitpython_ra8875.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/adafruit_ra8875/ra8875.py` & `adafruit-circuitpython-ra8875-3.1.9/adafruit_ra8875/ra8875.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/adafruit_ra8875/registers.py` & `adafruit-circuitpython-ra8875-3.1.9/adafruit_ra8875/registers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ra8875-3.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/docs/conf.py` & `adafruit-circuitpython-ra8875-3.1.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 # autodoc_mock_imports = ["digitalio", "busio"]
 
 
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

### Comparing `adafruit-circuitpython-ra8875-3.1.8/docs/index.rst` & `adafruit-circuitpython-ra8875-3.1.9/docs/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     RA8875 Driver Board for 40-pin TFT Touch Displays - 800x480 <https://www.adafruit.com/product/1590>
 
 .. toctree::
     :caption: Other Links
 
     Download <https://github.com/melissagirl/Adafruit_CircuitPython_RA8875/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-ra8875-3.1.8/examples/ra8875_blinka.bmp` & `adafruit-circuitpython-ra8875-3.1.9/examples/ra8875_blinka.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/examples/ra8875_bmptest.py` & `adafruit-circuitpython-ra8875-3.1.9/examples/ra8875_bmptest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/examples/ra8875_simpletest.py` & `adafruit-circuitpython-ra8875-3.1.9/examples/ra8875_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ra8875-3.1.8/setup.py` & `adafruit-circuitpython-ra8875-3.1.9/setup.py`

 * *Files 6% similar despite different names*

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
     keywords="adafruit ra8875 display driver tft touch screen hardware micropython circuitpython",
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     packages=["adafruit_ra8875"],
 )
```

