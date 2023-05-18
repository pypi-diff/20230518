# Comparing `tmp/adafruit-circuitpython-matrixportal-3.0.8.tar.gz` & `tmp/adafruit-circuitpython-matrixportal-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-matrixportal-3.0.8.tar", last modified: Tue Aug  9 19:30:24 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-matrixportal-3.0.9.tar", last modified: Mon Aug 22 19:00:13 2022, max compression
```

## Comparing `adafruit-circuitpython-matrixportal-3.0.8.tar` & `adafruit-circuitpython-matrixportal-3.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:30:24.080548 adafruit-circuitpython-matrixportal-3.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:30:24.076548 adafruit-circuitpython-matrixportal-3.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:30:24.076548 adafruit-circuitpython-matrixportal-3.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:30:24.076548 adafruit-circuitpython-matrixportal-3.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:30:24.076548 adafruit-circuitpython-matrixportal-3.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-08-09 19:30:24.080548 adafruit-circuitpython-matrixportal-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:30:24.076548 adafruit-circuitpython-matrixportal-3.0.8/adafruit_circuitpython_matrixportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-08-09 19:30:24.000000 adafruit-circuitpython-matrixportal-3.0.8/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-08-09 19:30:24.000000 adafruit-circuitpython-matrixportal-3.0.8/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:30:24.000000 adafruit-circuitpython-matrixportal-3.0.8/adafruit_circuitpython_matrixportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-08-09 19:30:24.000000 adafruit-circuitpython-matrixportal-3.0.8/adafruit_circuitpython_matrixportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-09 19:30:24.000000 adafruit-circuitpython-matrixportal-3.0.8/adafruit_circuitpython_matrixportal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:30:24.076548 adafruit-circuitpython-matrixportal-3.0.8/adafruit_matrixportal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 19:30:16.000000 adafruit-circuitpython-matrixportal-3.0.8/adafruit_matrixportal/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2575 2022-08-09 19:30:16.000000 adafruit-circuitpython-matrixportal-3.0.8/adafruit_matrixportal/graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7726 2022-08-09 19:30:16.000000 adafruit-circuitpython-matrixportal-3.0.8/adafruit_matrixportal/matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10453 2022-08-09 19:30:16.000000 adafruit-circuitpython-matrixportal-3.0.8/adafruit_matrixportal/matrixportal.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2750 2022-08-09 19:30:16.000000 adafruit-circuitpython-matrixportal-3.0.8/adafruit_matrixportal/network.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:30:24.076548 adafruit-circuitpython-matrixportal-3.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:30:24.080548 adafruit-circuitpython-matrixportal-3.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5554 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:30:24.080548 adafruit-circuitpython-matrixportal-3.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-08-09 19:30:16.000000 adafruit-circuitpython-matrixportal-3.0.8/examples/matrixportal_scrolling_bitcoin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-08-09 19:30:16.000000 adafruit-circuitpython-matrixportal-3.0.8/examples/matrixportal_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-08-09 19:30:16.000000 adafruit-circuitpython-matrixportal-3.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-08-09 19:30:08.000000 adafruit-circuitpython-matrixportal-3.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:30:24.080548 adafruit-circuitpython-matrixportal-3.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.624096 adafruit-circuitpython-matrixportal-3.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.604096 adafruit-circuitpython-matrixportal-3.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.612096 adafruit-circuitpython-matrixportal-3.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.612096 adafruit-circuitpython-matrixportal-3.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.612096 adafruit-circuitpython-matrixportal-3.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-08-22 19:00:13.624096 adafruit-circuitpython-matrixportal-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2769 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.616096 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-08-22 19:00:13.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-08-22 19:00:13.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 19:00:13.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-08-22 19:00:13.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-22 19:00:13.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.616096 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2575 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7726 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10453 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/matrixportal.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2750 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/network.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.620096 adafruit-circuitpython-matrixportal-3.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.620096 adafruit-circuitpython-matrixportal-3.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5554 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:00:13.624096 adafruit-circuitpython-matrixportal-3.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/examples/matrixportal_scrolling_bitcoin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/examples/matrixportal_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-08-22 19:00:03.000000 adafruit-circuitpython-matrixportal-3.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-08-22 18:59:53.000000 adafruit-circuitpython-matrixportal-3.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 19:00:13.624096 adafruit-circuitpython-matrixportal-3.0.9/setup.cfg
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-matrixportal-3.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-matrixportal-3.0.9/.github/workflows/build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -67,11 +67,11 @@
       run: |
         echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
         pip install --upgrade build twine
         for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
-            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+            sed -i -e "s/0.0.0+auto.0/1.2.3/" $file;
         done;
         python -m build
         twine check dist/*
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-matrixportal-3.0.9/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -78,11 +78,11 @@
     - name: Build and publish
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       env:
         TWINE_USERNAME: ${{ secrets.pypi_username }}
         TWINE_PASSWORD: ${{ secrets.pypi_password }}
       run: |
         for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
-            sed -i -e "s/0.0.0-auto.0/${{github.event.release.tag_name}}/" $file;
+            sed -i -e "s/0.0.0+auto.0/${{github.event.release.tag_name}}/" $file;
         done;
         python -m build
         twine upload dist/*
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/.gitignore` & `adafruit-circuitpython-matrixportal-3.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-matrixportal-3.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/.pylintrc` & `adafruit-circuitpython-matrixportal-3.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-matrixportal-3.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/LICENSE` & `adafruit-circuitpython-matrixportal-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-matrixportal-3.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-matrixportal-3.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-matrixportal-3.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/PKG-INFO` & `adafruit-circuitpython-matrixportal-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-matrixportal
-Version: 3.0.8
+Version: 3.0.9
 Summary: CircuitPython helper for Adafruit MatrixPortal M4, Adafruit RGB Matrix Shield + Metro M4 Airlift Lite, and Adafruit RGB Matrix FeatherWings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal
 Keywords: adafruit,matrixportal,matrix,rgb,led,feather,featherwing,shieldbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/README.rst` & `adafruit-circuitpython-matrixportal-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO` & `adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-matrixportal
-Version: 3.0.8
+Version: 3.0.9
 Summary: CircuitPython helper for Adafruit MatrixPortal M4, Adafruit RGB Matrix Shield + Metro M4 Airlift Lite, and Adafruit RGB Matrix FeatherWings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal
 Keywords: adafruit,matrixportal,matrix,rgb,led,feather,featherwing,shieldbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt` & `adafruit-circuitpython-matrixportal-3.0.9/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/adafruit_matrixportal/graphics.py` & `adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/graphics.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 from adafruit_portalbase.graphics import GraphicsBase
 from adafruit_matrixportal.matrix import Matrix
 
-__version__ = "3.0.8"
+__version__ = "3.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class Graphics(GraphicsBase):
     """Graphics Helper Class for the MatrixPortal Library
 
     :param default_bg: The path to your default background image file or a hex color.
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/adafruit_matrixportal/matrix.py` & `adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import os
 import board
 import displayio
 import rgbmatrix
 import framebufferio
 
 
-__version__ = "3.0.8"
+__version__ = "3.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class Matrix:
     """Class representing the Adafruit RGB Matrix. This is used to automatically
     initialize the display.
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/adafruit_matrixportal/matrixportal.py` & `adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/matrixportal.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import gc
 from time import sleep
 import terminalio
 from adafruit_portalbase import PortalBase
 from adafruit_matrixportal.network import Network
 from adafruit_matrixportal.graphics import Graphics
 
-__version__ = "3.0.8"
+__version__ = "3.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class MatrixPortal(PortalBase):
     """Class representing the Adafruit RGB Matrix Portal.
 
     :param url: The URL of your data source. Defaults to ``None``.
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/adafruit_matrixportal/network.py` & `adafruit-circuitpython-matrixportal-3.0.9/adafruit_matrixportal/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 """
 
 import gc
 import neopixel
 from adafruit_portalbase.network import NetworkBase
 from adafruit_portalbase.wifi_coprocessor import WiFi
 
-__version__ = "3.0.8"
+__version__ = "3.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class Network(NetworkBase):
     """Class representing the Adafruit RGB Matrix Portal.
 
     :param status_neopixel: The pin for the status NeoPixel. Use ``board.NEOPIXEL`` for the on-board
```

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-matrixportal-3.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/docs/conf.py` & `adafruit-circuitpython-matrixportal-3.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/docs/index.rst` & `adafruit-circuitpython-matrixportal-3.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/examples/matrixportal_scrolling_bitcoin.py` & `adafruit-circuitpython-matrixportal-3.0.9/examples/matrixportal_scrolling_bitcoin.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/examples/matrixportal_simpletest.py` & `adafruit-circuitpython-matrixportal-3.0.9/examples/matrixportal_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.0.8/pyproject.toml` & `adafruit-circuitpython-matrixportal-3.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-matrixportal"
 description = "CircuitPython helper for Adafruit MatrixPortal M4, Adafruit RGB Matrix Shield + Metro M4 Airlift Lite, and Adafruit RGB Matrix FeatherWings"
-version = "3.0.8"
+version = "3.0.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal"}
 keywords = [
     "adafruit",
```

