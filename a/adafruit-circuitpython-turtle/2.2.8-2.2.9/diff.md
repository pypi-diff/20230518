# Comparing `tmp/adafruit-circuitpython-turtle-2.2.8.tar.gz` & `tmp/adafruit-circuitpython-turtle-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-turtle-2.2.8.tar", last modified: Tue Aug  9 19:40:56 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-turtle-2.2.9.tar", last modified: Mon Aug 22 19:02:27 2022, max compression
```

## Comparing `adafruit-circuitpython-turtle-2.2.8.tar` & `adafruit-circuitpython-turtle-2.2.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.205923 adafruit-circuitpython-turtle-2.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.201923 adafruit-circuitpython-turtle-2.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.201923 adafruit-circuitpython-turtle-2.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.201923 adafruit-circuitpython-turtle-2.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.201923 adafruit-circuitpython-turtle-2.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-08-09 19:40:56.205923 adafruit-circuitpython-turtle-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3081 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.205923 adafruit-circuitpython-turtle-2.2.8/adafruit_circuitpython_turtle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-08-09 19:40:56.000000 adafruit-circuitpython-turtle-2.2.8/adafruit_circuitpython_turtle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-08-09 19:40:56.000000 adafruit-circuitpython-turtle-2.2.8/adafruit_circuitpython_turtle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:40:56.000000 adafruit-circuitpython-turtle-2.2.8/adafruit_circuitpython_turtle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-09 19:40:56.000000 adafruit-circuitpython-turtle-2.2.8/adafruit_circuitpython_turtle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-09 19:40:56.000000 adafruit-circuitpython-turtle-2.2.8/adafruit_circuitpython_turtle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    38093 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/adafruit_turtle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.205923 adafruit-circuitpython-turtle-2.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.205923 adafruit-circuitpython-turtle-2.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5861 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.205923 adafruit-circuitpython-turtle-2.2.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.205923 adafruit-circuitpython-turtle-2.2.8/examples/icons/
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/examples/icons/Play_48x48_small.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/examples/icons/Play_48x48_small.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_benzene.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_bgpic_changeturtle.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_circle.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_circle_hex.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_dots.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_hilbert.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_koch.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_manual_hex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_overlayed_koch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_sierpinski.py
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_square.py
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_star.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/examples/turtle_swirl.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-08-09 19:40:48.000000 adafruit-circuitpython-turtle-2.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-09 19:40:39.000000 adafruit-circuitpython-turtle-2.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:40:56.205923 adafruit-circuitpython-turtle-2.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:27.177047 adafruit-circuitpython-turtle-2.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:27.169047 adafruit-circuitpython-turtle-2.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:27.173047 adafruit-circuitpython-turtle-2.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:27.173047 adafruit-circuitpython-turtle-2.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:27.173047 adafruit-circuitpython-turtle-2.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-08-22 19:02:27.177047 adafruit-circuitpython-turtle-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3081 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:27.173047 adafruit-circuitpython-turtle-2.2.9/adafruit_circuitpython_turtle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-08-22 19:02:27.000000 adafruit-circuitpython-turtle-2.2.9/adafruit_circuitpython_turtle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-08-22 19:02:27.000000 adafruit-circuitpython-turtle-2.2.9/adafruit_circuitpython_turtle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 19:02:27.000000 adafruit-circuitpython-turtle-2.2.9/adafruit_circuitpython_turtle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-22 19:02:27.000000 adafruit-circuitpython-turtle-2.2.9/adafruit_circuitpython_turtle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-22 19:02:27.000000 adafruit-circuitpython-turtle-2.2.9/adafruit_circuitpython_turtle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    38093 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/adafruit_turtle.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:27.173047 adafruit-circuitpython-turtle-2.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:27.173047 adafruit-circuitpython-turtle-2.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5861 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:27.173047 adafruit-circuitpython-turtle-2.2.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:27.173047 adafruit-circuitpython-turtle-2.2.9/examples/icons/
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/examples/icons/Play_48x48_small.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/examples/icons/Play_48x48_small.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_benzene.py
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_bgpic_changeturtle.py
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_circle.py
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_circle_hex.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_dots.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_hilbert.py
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_koch.py
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_manual_hex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_overlayed_koch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_sierpinski.py
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_square.py
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_star.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/examples/turtle_swirl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-08-22 19:02:18.000000 adafruit-circuitpython-turtle-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-22 19:02:10.000000 adafruit-circuitpython-turtle-2.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 19:02:27.177047 adafruit-circuitpython-turtle-2.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-turtle-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-turtle-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-turtle-2.2.9/.github/workflows/build.yml`

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

### Comparing `adafruit-circuitpython-turtle-2.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-turtle-2.2.9/.github/workflows/release.yml`

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

### Comparing `adafruit-circuitpython-turtle-2.2.8/.gitignore` & `adafruit-circuitpython-turtle-2.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-turtle-2.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/.pylintrc` & `adafruit-circuitpython-turtle-2.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-turtle-2.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/LICENSE` & `adafruit-circuitpython-turtle-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-turtle-2.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-turtle-2.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-turtle-2.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/PKG-INFO` & `adafruit-circuitpython-turtle-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-turtle
-Version: 2.2.8
+Version: 2.2.9
 Summary: Turtle graphics library for CircuitPython and displayio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_turtle
 Keywords: adafruit,blinka,circuitpython,micropython,turtle,graphics,turtle
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-turtle-2.2.8/README.rst` & `adafruit-circuitpython-turtle-2.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/adafruit_circuitpython_turtle.egg-info/PKG-INFO` & `adafruit-circuitpython-turtle-2.2.9/adafruit_circuitpython_turtle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-turtle
-Version: 2.2.8
+Version: 2.2.9
 Summary: Turtle graphics library for CircuitPython and displayio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_turtle
 Keywords: adafruit,blinka,circuitpython,micropython,turtle,graphics,turtle
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-turtle-2.2.8/adafruit_circuitpython_turtle.egg-info/SOURCES.txt` & `adafruit-circuitpython-turtle-2.2.9/adafruit_circuitpython_turtle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/adafruit_turtle.py` & `adafruit-circuitpython-turtle-2.2.9/adafruit_turtle.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 import gc
 import math
 import time
 import board
 import displayio
 
-__version__ = "2.2.8"
+__version__ = "2.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_turtle.git"
 
 
 class Color:
     """Standard colors"""
 
     WHITE = 0xFFFFFF
```

### Comparing `adafruit-circuitpython-turtle-2.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-turtle-2.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/docs/conf.py` & `adafruit-circuitpython-turtle-2.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/docs/index.rst` & `adafruit-circuitpython-turtle-2.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/examples/icons/Play_48x48_small.bmp` & `adafruit-circuitpython-turtle-2.2.9/examples/icons/Play_48x48_small.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/examples/turtle_benzene.py` & `adafruit-circuitpython-turtle-2.2.9/examples/turtle_benzene.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/examples/turtle_bgpic_changeturtle.py` & `adafruit-circuitpython-turtle-2.2.9/examples/turtle_bgpic_changeturtle.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/examples/turtle_hilbert.py` & `adafruit-circuitpython-turtle-2.2.9/examples/turtle_hilbert.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/examples/turtle_koch.py` & `adafruit-circuitpython-turtle-2.2.9/examples/turtle_koch.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/examples/turtle_overlayed_koch.py` & `adafruit-circuitpython-turtle-2.2.9/examples/turtle_overlayed_koch.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/examples/turtle_sierpinski.py` & `adafruit-circuitpython-turtle-2.2.9/examples/turtle_sierpinski.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/examples/turtle_simpletest.py` & `adafruit-circuitpython-turtle-2.2.9/examples/turtle_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/examples/turtle_star.py` & `adafruit-circuitpython-turtle-2.2.9/examples/turtle_star.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-turtle-2.2.8/pyproject.toml` & `adafruit-circuitpython-turtle-2.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-turtle"
 description = "Turtle graphics library for CircuitPython and displayio"
-version = "2.2.8"
+version = "2.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_turtle"}
 keywords = [
     "adafruit",
```

