# Comparing `tmp/adafruit-circuitpython-led-animation-2.7.0.tar.gz` & `tmp/adafruit-circuitpython-led-animation-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-led-animation-2.7.0.tar", last modified: Mon Feb 27 14:59:00 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-led-animation-2.7.1.tar", last modified: Thu May 18 15:38:20 2023, max compression
```

## Comparing `adafruit-circuitpython-led-animation-2.7.0.tar` & `adafruit-circuitpython-led-animation-2.7.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:59:00.576175 adafruit-circuitpython-led-animation-2.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:59:00.560175 adafruit-circuitpython-led-animation-2.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:59:00.560175 adafruit-circuitpython-led-animation-2.7.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:59:00.564175 adafruit-circuitpython-led-animation-2.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:59:00.564175 adafruit-circuitpython-led-animation-2.7.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-02-27 14:59:00.572175 adafruit-circuitpython-led-animation-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:59:00.564175 adafruit-circuitpython-led-animation-2.7.0/adafruit_circuitpython_led_animation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-02-27 14:59:00.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_circuitpython_led_animation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-02-27 14:59:00.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_circuitpython_led_animation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 14:59:00.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_circuitpython_led_animation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-27 14:59:00.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_circuitpython_led_animation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-27 14:59:00.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_circuitpython_led_animation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:59:00.564175 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:59:00.568175 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/blink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/chase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/colorcycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/customcolorchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/grid_rain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/multicolor_comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/pulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/rainbow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/rainbowchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/rainbowcomet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/rainbowsparkle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/solid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/sparkle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/sparklepulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:59:00.568175 adafruit-circuitpython-led-animation-2.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:59:00.568175 adafruit-circuitpython-led-animation-2.7.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 14:59:00.572175 adafruit-circuitpython-led-animation-2.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_all_animations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_basic_animations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_blink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_chase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_customcolorchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_cycle_animations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_freeze_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_multicolor_comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_pixel_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_rainbow_animations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_resume_animation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_samd21_reset_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_sparkle_animations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_sparkle_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-27 14:58:50.000000 adafruit-circuitpython-led-animation-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-27 14:58:34.000000 adafruit-circuitpython-led-animation-2.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 14:59:00.576175 adafruit-circuitpython-led-animation-2.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:20.364305 adafruit-circuitpython-led-animation-2.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:20.348305 adafruit-circuitpython-led-animation-2.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:20.352305 adafruit-circuitpython-led-animation-2.7.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:20.352305 adafruit-circuitpython-led-animation-2.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:20.352305 adafruit-circuitpython-led-animation-2.7.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-18 15:38:20.364305 adafruit-circuitpython-led-animation-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:20.352305 adafruit-circuitpython-led-animation-2.7.1/adafruit_circuitpython_led_animation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-18 15:38:20.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_circuitpython_led_animation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-18 15:38:20.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_circuitpython_led_animation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:38:20.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_circuitpython_led_animation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:38:20.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_circuitpython_led_animation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 15:38:20.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_circuitpython_led_animation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:20.356305 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:20.356305 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/blink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/chase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/colorcycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/customcolorchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/grid_rain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/multicolor_comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/pulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/rainbowchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/rainbowcomet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/rainbowsparkle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/solid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/sparkle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/sparklepulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:20.360305 adafruit-circuitpython-led-animation-2.7.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:20.360305 adafruit-circuitpython-led-animation-2.7.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:20.364305 adafruit-circuitpython-led-animation-2.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_all_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_basic_animations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_blink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_chase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_customcolorchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_cycle_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_freeze_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_multicolor_comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_pixel_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_rainbow_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_resume_animation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_samd21_reset_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_sparkle_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_sparkle_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-18 15:38:09.000000 adafruit-circuitpython-led-animation-2.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 15:37:51.000000 adafruit-circuitpython-led-animation-2.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:38:20.364305 adafruit-circuitpython-led-animation-2.7.1/setup.cfg
```

### Comparing `adafruit-circuitpython-led-animation-2.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-led-animation-2.7.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/.gitignore` & `adafruit-circuitpython-led-animation-2.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/.pre-commit-config.yaml` & `adafruit-circuitpython-led-animation-2.7.1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-led-animation-2.7.0/.pylintrc` & `adafruit-circuitpython-led-animation-2.7.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-led-animation-2.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/LICENSE` & `adafruit-circuitpython-led-animation-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-led-animation-2.7.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/LICENSES/MIT.txt` & `adafruit-circuitpython-led-animation-2.7.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-led-animation-2.7.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/PKG-INFO` & `adafruit-circuitpython-led-animation-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-led-animation
-Version: 2.7.0
+Version: 2.7.1
 Summary: CircuitPython helper for LED colors and animations.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation
 Keywords: adafruit,blinka,circuitpython,micropython,led,animation,led,colors,animations
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-led-animation-2.7.0/README.rst` & `adafruit-circuitpython-led-animation-2.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_circuitpython_led_animation.egg-info/PKG-INFO` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_circuitpython_led_animation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-led-animation
-Version: 2.7.0
+Version: 2.7.1
 Summary: CircuitPython helper for LED colors and animations.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation
 Keywords: adafruit,blinka,circuitpython,micropython,led,animation,led,colors,animations
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_circuitpython_led_animation.egg-info/SOURCES.txt` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_circuitpython_led_animation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/__init__.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/__init__.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
-__version__ = "2.7.0"
+__version__ = "2.7.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 from adafruit_led_animation import MS_PER_SECOND, monotonic_ms
 
 
 class Animation:
     # pylint: disable=too-many-instance-attributes
```

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/blink.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/blink.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/chase.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/chase.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/colorcycle.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/colorcycle.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/comet.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/comet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/customcolorchase.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/customcolorchase.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/grid_rain.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/grid_rain.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   https://circuitpython.org/downloads
 
 """
 
 import random
 from adafruit_led_animation.animation import Animation
 
-__version__ = "2.7.0"
+__version__ = "2.7.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 from adafruit_led_animation.color import BLACK, colorwheel, calculate_intensity, GREEN
 
 
 class Rain(Animation):
     """
@@ -53,15 +53,14 @@
         self._count = count
         self._length = length
         self._background = background
         self._raindrops = []
         super().__init__(grid_object, speed, color, name=name)
 
     def draw(self):
-
         # Move raindrops down
         keep = []
         for raindrop in self._raindrops:
             pixels = []
             if raindrop[1][0][0] >= 0:
                 self.pixel_object[raindrop[0], raindrop[1][0][0]] = self._background
             for pixel in raindrop[1]:
```

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/multicolor_comet.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/multicolor_comet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/pulse.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/pulse.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/rainbow.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/rainbow.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 """
 
 from adafruit_led_animation.animation import Animation
 from adafruit_led_animation.color import BLACK, colorwheel
 from adafruit_led_animation import MS_PER_SECOND, monotonic_ms
 
-__version__ = "2.7.0"
+__version__ = "2.7.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 
 class Rainbow(Animation):
     """
     The classic rainbow color wheel.
```

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/rainbowchase.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/rainbowchase.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/rainbowcomet.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/rainbowcomet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/rainbowsparkle.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/rainbowsparkle.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/solid.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/solid.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/sparkle.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/sparkle.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   https://circuitpython.org/downloads
 
 """
 
 import random
 from adafruit_led_animation.animation import Animation
 
-__version__ = "2.7.0"
+__version__ = "2.7.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 
 class Sparkle(Animation):
     """
     Sparkle animation of a single color.
```

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/animation/sparklepulse.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/animation/sparklepulse.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/color.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/color.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/grid.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/grid.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/group.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
-__version__ = "2.7.0"
+__version__ = "2.7.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 from adafruit_led_animation.animation import Animation
 
 
 class AnimationGroup:
     """
```

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/helper.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/helper.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/adafruit_led_animation/sequence.py` & `adafruit-circuitpython-led-animation-2.7.1/adafruit_led_animation/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 """
 
 import random
 from adafruit_led_animation.color import BLACK
 from . import MS_PER_SECOND, monotonic_ms
 
-__version__ = "2.7.0"
+__version__ = "2.7.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation.git"
 
 
 class AnimationSequence:
     """
     A sequence of Animations to run in succession, looping forever.
     Advances manually, or at the specified interval.
```

### Comparing `adafruit-circuitpython-led-animation-2.7.0/docs/_static/favicon.ico` & `adafruit-circuitpython-led-animation-2.7.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/docs/api.rst` & `adafruit-circuitpython-led-animation-2.7.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/docs/conf.py` & `adafruit-circuitpython-led-animation-2.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/docs/examples.rst` & `adafruit-circuitpython-led-animation-2.7.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/docs/index.rst` & `adafruit-circuitpython-led-animation-2.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_all_animations.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_all_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_basic_animations.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_basic_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_blink.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_blink.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_chase.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_chase.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_comet.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_comet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_customcolorchase.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_customcolorchase.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_cycle_animations.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_cycle_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_freeze_animation.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_freeze_animation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_group.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_group.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_multicolor_comet.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_multicolor_comet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_pixel_map.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_pixel_map.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_rainbow_animations.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_rainbow_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_resume_animation.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_resume_animation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_samd21_reset_interval.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_samd21_reset_interval.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_sequence.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_sequence.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_simpletest.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_sparkle_animations.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_sparkle_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/examples/led_animation_sparkle_mask.py` & `adafruit-circuitpython-led-animation-2.7.1/examples/led_animation_sparkle_mask.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-led-animation-2.7.0/pyproject.toml` & `adafruit-circuitpython-led-animation-2.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-led-animation"
 description = "CircuitPython helper for LED colors and animations."
-version = "2.7.0"
+version = "2.7.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_LED_Animation"}
 keywords = [
     "adafruit",
```

