# Comparing `tmp/adafruit-circuitpython-progressbar-2.3.8.tar.gz` & `tmp/adafruit-circuitpython-progressbar-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-progressbar-2.3.8.tar", last modified: Fri Aug 26 02:47:47 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-progressbar-2.3.9.tar", last modified: Tue Nov 15 18:12:01 2022, max compression
```

## Comparing `adafruit-circuitpython-progressbar-2.3.8.tar` & `adafruit-circuitpython-progressbar-2.3.9.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:47:47.689992 adafruit-circuitpython-progressbar-2.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:47:47.681992 adafruit-circuitpython-progressbar-2.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:47:47.681992 adafruit-circuitpython-progressbar-2.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:47:47.681992 adafruit-circuitpython-progressbar-2.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16253 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:47:47.685992 adafruit-circuitpython-progressbar-2.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-08-26 02:47:47.689992 adafruit-circuitpython-progressbar-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2526 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:47:47.685992 adafruit-circuitpython-progressbar-2.3.8/adafruit_circuitpython_progressbar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-08-26 02:47:47.000000 adafruit-circuitpython-progressbar-2.3.8/adafruit_circuitpython_progressbar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-08-26 02:47:47.000000 adafruit-circuitpython-progressbar-2.3.8/adafruit_circuitpython_progressbar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:47:47.000000 adafruit-circuitpython-progressbar-2.3.8/adafruit_circuitpython_progressbar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-08-26 02:47:47.000000 adafruit-circuitpython-progressbar-2.3.8/adafruit_circuitpython_progressbar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-26 02:47:47.000000 adafruit-circuitpython-progressbar-2.3.8/adafruit_circuitpython_progressbar.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:47:47.685992 adafruit-circuitpython-progressbar-2.3.8/adafruit_progressbar/
--rwxr-xr-x   0 runner    (1001) docker     (121)    20618 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/adafruit_progressbar/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6342 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/adafruit_progressbar/horizontalprogressbar.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3100 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/adafruit_progressbar/progressbar.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5191 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/adafruit_progressbar/verticalprogressbar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:47:47.685992 adafruit-circuitpython-progressbar-2.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:47:47.685992 adafruit-circuitpython-progressbar-2.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5653 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:47:47.689992 adafruit-circuitpython-progressbar-2.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     7585 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_accelerometer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_combined.py
--rw-r--r--   0 runner    (1001) docker     (121)     3412 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_displayio_blinka.py
--rw-r--r--   0 runner    (1001) docker     (121)     2511 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_displayio_blinka_color_scale.py
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_magtag_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5038 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_matrixportal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_vertical_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-08-26 02:47:36.000000 adafruit-circuitpython-progressbar-2.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-08-26 02:47:26.000000 adafruit-circuitpython-progressbar-2.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:47:47.689992 adafruit-circuitpython-progressbar-2.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 18:12:01.253749 adafruit-circuitpython-progressbar-2.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 18:12:01.249749 adafruit-circuitpython-progressbar-2.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 18:12:01.249749 adafruit-circuitpython-progressbar-2.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 18:12:01.253749 adafruit-circuitpython-progressbar-2.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 18:12:01.253749 adafruit-circuitpython-progressbar-2.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-11-15 18:12:01.253749 adafruit-circuitpython-progressbar-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2526 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 18:12:01.253749 adafruit-circuitpython-progressbar-2.3.9/adafruit_circuitpython_progressbar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-11-15 18:12:01.000000 adafruit-circuitpython-progressbar-2.3.9/adafruit_circuitpython_progressbar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-11-15 18:12:01.000000 adafruit-circuitpython-progressbar-2.3.9/adafruit_circuitpython_progressbar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 18:12:01.000000 adafruit-circuitpython-progressbar-2.3.9/adafruit_circuitpython_progressbar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-15 18:12:01.000000 adafruit-circuitpython-progressbar-2.3.9/adafruit_circuitpython_progressbar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-15 18:12:01.000000 adafruit-circuitpython-progressbar-2.3.9/adafruit_circuitpython_progressbar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 18:12:01.253749 adafruit-circuitpython-progressbar-2.3.9/adafruit_progressbar/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    20672 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/adafruit_progressbar/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6342 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/adafruit_progressbar/horizontalprogressbar.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3100 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/adafruit_progressbar/progressbar.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5191 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/adafruit_progressbar/verticalprogressbar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 18:12:01.253749 adafruit-circuitpython-progressbar-2.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 18:12:01.253749 adafruit-circuitpython-progressbar-2.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      649 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5653 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 18:12:01.253749 adafruit-circuitpython-progressbar-2.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     7585 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_accelerometer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_combined.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3412 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_displayio_blinka.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2511 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_displayio_blinka_color_scale.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_magtag_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5038 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_matrixportal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_vertical_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-11-15 18:11:53.000000 adafruit-circuitpython-progressbar-2.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-15 18:11:42.000000 adafruit-circuitpython-progressbar-2.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 18:12:01.253749 adafruit-circuitpython-progressbar-2.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-progressbar-2.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-progressbar-2.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/.gitignore` & `adafruit-circuitpython-progressbar-2.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-progressbar-2.3.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-progressbar-2.3.8/.pylintrc` & `adafruit-circuitpython-progressbar-2.3.9/.pylintrc`

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
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -155,15 +155,15 @@
 # qualified names.
 ignored-classes=optparse.Values,thread._local,_thread._local
 
 # List of module names for which member attributes should not be checked
 # (useful for modules/projects where namespaces are manipulated during runtime
 # and thus existing member attributes cannot be deduced by static analysis. It
 # supports qualified module names, as well as Unix pattern matching.
-ignored-modules=board,time
+ignored-modules=board
 
 # Show a hint with possible names when a member name was not found. The aspect
 # of finding the hint is based on edit distance.
 missing-member-hint=yes
 
 # The minimum edit distance a name should have in order to be considered a
 # similar match for a missing member name.
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

### Comparing `adafruit-circuitpython-progressbar-2.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-progressbar-2.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/LICENSE` & `adafruit-circuitpython-progressbar-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-progressbar-2.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-progressbar-2.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-progressbar-2.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/PKG-INFO` & `adafruit-circuitpython-progressbar-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-progressbar
-Version: 2.3.8
+Version: 2.3.9
 Summary: Dynamic progress bar widget for CircuitPython displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ProgressBar
 Keywords: adafruit,blinka,circuitpython,micropython,progressbar,widget,,displayio,,progress,,bar,,element
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-progressbar-2.3.8/README.rst` & `adafruit-circuitpython-progressbar-2.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/adafruit_circuitpython_progressbar.egg-info/PKG-INFO` & `adafruit-circuitpython-progressbar-2.3.9/adafruit_circuitpython_progressbar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-progressbar
-Version: 2.3.8
+Version: 2.3.9
 Summary: Dynamic progress bar widget for CircuitPython displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ProgressBar
 Keywords: adafruit,blinka,circuitpython,micropython,progressbar,widget,,displayio,,progress,,bar,,element
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-progressbar-2.3.8/adafruit_circuitpython_progressbar.egg-info/SOURCES.txt` & `adafruit-circuitpython-progressbar-2.3.9/adafruit_circuitpython_progressbar.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 README.rst.license
 optional_requirements.txt
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
 adafruit_circuitpython_progressbar.egg-info/PKG-INFO
 adafruit_circuitpython_progressbar.egg-info/SOURCES.txt
 adafruit_circuitpython_progressbar.egg-info/dependency_links.txt
 adafruit_circuitpython_progressbar.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-progressbar-2.3.8/adafruit_progressbar/__init__.py` & `adafruit-circuitpython-progressbar-2.3.9/adafruit_progressbar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # imports
 try:
     from typing import Tuple, Union, List
 except ImportError:
     pass  # No harm if the module isn't located
 import displayio
 
-__version__ = "2.3.8"
+__version__ = "2.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ProgressBar.git"
 
 
 class ProgressBarBase(displayio.TileGrid):
     """The base class for dynamic progress bar widgets.
 
     :param position: The coordinates (x, y) of the top left corner
@@ -486,20 +486,20 @@
         """
 
         if self.maximum == self.minimum:
             return 0.0
 
         return (float(value) - self.minimum) / (self.maximum - self.minimum)
 
-    @classmethod
-    def _get_value_sizes(cls, _old_ratio: float, _new_ratio: float) -> Tuple[int, int]:
+    # pylint: disable=no-self-use
+    def _get_value_sizes(self, _old_ratio: float, _new_ratio: float) -> Tuple[int, int]:
         return 0, 0
 
-    @classmethod
-    def _get_max_fill_size(cls) -> int:
+    # pylint: disable=no-self-use
+    def _get_max_fill_size(self) -> int:
         return 0
 
     def _get_ratios(
         self, _old_value: Union[int, float], _new_value: Union[int, float]
     ) -> Tuple[float, float]:
         return self.get_value_ratio(_old_value), self.get_value_ratio(_new_value)
 
@@ -517,16 +517,16 @@
             _new_value_size -= 1
 
         return _new_value_size
 
     def _get_sizes_min_max(self) -> Tuple[int, int]:
         return 0, min(self.fill_width(), self.fill_height())
 
-    @classmethod
-    def _invert_fill_direction(cls) -> bool:
+    # pylint: disable=no-self-use
+    def _invert_fill_direction(self) -> bool:
         return False
 
     def _get_horizontal_fill(
         self, _start: int, _end: int, _incr: int
     ) -> Tuple[int, int, int]:
         return 0, self.fill_width(), 1  # Subclass must return values
```

### Comparing `adafruit-circuitpython-progressbar-2.3.8/adafruit_progressbar/horizontalprogressbar.py` & `adafruit-circuitpython-progressbar-2.3.9/adafruit_progressbar/horizontalprogressbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 try:
     from typing import Tuple, Union
 except ImportError:
     pass  # Not needed for execution
 from . import ProgressBarBase
 
-__version__ = "2.3.8"
+__version__ = "2.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ProgressBar.git"
 
 
 # pylint: disable=too-few-public-methods
 class HorizontalFillDirection:
     """This enum is used to specify the direction in which the progress
     bar's display bar should fill as the value represented increases."""
```

### Comparing `adafruit-circuitpython-progressbar-2.3.8/adafruit_progressbar/progressbar.py` & `adafruit-circuitpython-progressbar-2.3.9/adafruit_progressbar/progressbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 # imports
 from adafruit_progressbar.horizontalprogressbar import HorizontalProgressBar
 
-__version__ = "2.3.8"
+__version__ = "2.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ProgressBar.git"
 
 # pylint: disable=too-many-arguments, too-few-public-methods
 class ProgressBar(HorizontalProgressBar):
     """A dynamic progress bar widget.
 
     NOTE: This class is made available for backward compatibility with v1.x of
```

### Comparing `adafruit-circuitpython-progressbar-2.3.8/adafruit_progressbar/verticalprogressbar.py` & `adafruit-circuitpython-progressbar-2.3.9/adafruit_progressbar/verticalprogressbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Tuple
 except ImportError:
     pass  # Not needed for execution
 from . import ProgressBarBase
 from .horizontalprogressbar import HorizontalProgressBar
 
-__version__ = "2.3.8"
+__version__ = "2.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ProgressBar.git"
 
 # pylint: disable=too-few-public-methods
 class VerticalFillDirection:
     """This enum is used to specify the direction in which the progress
     bar's display bar should fill as the value represented increases."""
```

### Comparing `adafruit-circuitpython-progressbar-2.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-progressbar-2.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/docs/api.rst` & `adafruit-circuitpython-progressbar-2.3.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/docs/conf.py` & `adafruit-circuitpython-progressbar-2.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/docs/examples.rst` & `adafruit-circuitpython-progressbar-2.3.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/docs/index.rst` & `adafruit-circuitpython-progressbar-2.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_accelerometer.py` & `adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_accelerometer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_combined.py` & `adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_combined.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_displayio_blinka.py` & `adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_displayio_blinka.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_displayio_blinka_color_scale.py` & `adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_displayio_blinka_color_scale.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_magtag_simpletest.py` & `adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_magtag_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_matrixportal.py` & `adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_matrixportal.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_simpletest.py` & `adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/examples/progressbar_vertical_simpletest.py` & `adafruit-circuitpython-progressbar-2.3.9/examples/progressbar_vertical_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-progressbar-2.3.8/pyproject.toml` & `adafruit-circuitpython-progressbar-2.3.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-progressbar"
 description = "Dynamic progress bar widget for CircuitPython displays"
-version = "2.3.8"
+version = "2.3.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ProgressBar"}
 keywords = [
     "adafruit",
```

