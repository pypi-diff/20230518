# Comparing `tmp/adafruit-circuitpython-st7789-1.5.8.tar.gz` & `tmp/adafruit-circuitpython-st7789-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-st7789-1.5.8.tar", last modified: Mon May  2 21:47:51 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-st7789-1.5.9.tar", last modified: Tue Jun  7 17:02:48 2022, max compression
```

## Comparing `adafruit-circuitpython-st7789-1.5.8.tar` & `adafruit-circuitpython-st7789-1.5.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:47:51.134202 adafruit-circuitpython-st7789-1.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:47:51.126202 adafruit-circuitpython-st7789-1.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:47:51.130202 adafruit-circuitpython-st7789-1.5.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:47:51.130202 adafruit-circuitpython-st7789-1.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:47:51.130202 adafruit-circuitpython-st7789-1.5.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3281 2022-05-02 21:47:51.134202 adafruit-circuitpython-st7789-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:47:51.130202 adafruit-circuitpython-st7789-1.5.8/adafruit_circuitpython_st7789.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3281 2022-05-02 21:47:51.000000 adafruit-circuitpython-st7789-1.5.8/adafruit_circuitpython_st7789.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-05-02 21:47:51.000000 adafruit-circuitpython-st7789-1.5.8/adafruit_circuitpython_st7789.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-02 21:47:51.000000 adafruit-circuitpython-st7789-1.5.8/adafruit_circuitpython_st7789.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-02 21:47:51.000000 adafruit-circuitpython-st7789-1.5.8/adafruit_circuitpython_st7789.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-02 21:47:51.000000 adafruit-circuitpython-st7789-1.5.8/adafruit_circuitpython_st7789.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     1866 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/adafruit_st7789.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:47:51.130202 adafruit-circuitpython-st7789-1.5.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:47:51.134202 adafruit-circuitpython-st7789-1.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5481 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:47:51.134202 adafruit-circuitpython-st7789-1.5.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_170x320_1.9_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_172x320_1.47_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x135_pitft_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1915 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x135_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x135_simpletest_Pimoroni_Pico_Display_Pack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x240_bonnet_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x240_pitft_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x240_simpletest_Pimoroni_Pico_Explorer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x240_simpletest_Waveshare_PicoLCD_1_3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_280x240_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_320x240_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_320x240_simpletest_Pimoroni_Pico_Display_2_0.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/examples/st7789_tft_gizmo_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-02 21:47:51.134202 adafruit-circuitpython-st7789-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-05-02 21:47:36.000000 adafruit-circuitpython-st7789-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:48.675017 adafruit-circuitpython-st7789-1.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:48.667017 adafruit-circuitpython-st7789-1.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:48.667017 adafruit-circuitpython-st7789-1.5.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:48.667017 adafruit-circuitpython-st7789-1.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:48.667017 adafruit-circuitpython-st7789-1.5.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3281 2022-06-07 17:02:48.675017 adafruit-circuitpython-st7789-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:48.671017 adafruit-circuitpython-st7789-1.5.9/adafruit_circuitpython_st7789.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3281 2022-06-07 17:02:48.000000 adafruit-circuitpython-st7789-1.5.9/adafruit_circuitpython_st7789.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-06-07 17:02:48.000000 adafruit-circuitpython-st7789-1.5.9/adafruit_circuitpython_st7789.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:02:48.000000 adafruit-circuitpython-st7789-1.5.9/adafruit_circuitpython_st7789.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-07 17:02:48.000000 adafruit-circuitpython-st7789-1.5.9/adafruit_circuitpython_st7789.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 17:02:48.000000 adafruit-circuitpython-st7789-1.5.9/adafruit_circuitpython_st7789.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1866 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/adafruit_st7789.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:48.671017 adafruit-circuitpython-st7789-1.5.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:48.671017 adafruit-circuitpython-st7789-1.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5481 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:48.675017 adafruit-circuitpython-st7789-1.5.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_170x320_1.9_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_172x320_1.47_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x135_pitft_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1915 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x135_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x135_simpletest_Pimoroni_Pico_Display_Pack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x240_bonnet_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x240_pitft_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x240_simpletest_Pimoroni_Pico_Explorer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x240_simpletest_Waveshare_PicoLCD_1_3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_280x240_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_320x240_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_320x240_simpletest_Pimoroni_Pico_Display_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/examples/st7789_tft_gizmo_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:02:48.675017 adafruit-circuitpython-st7789-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-06-07 17:02:32.000000 adafruit-circuitpython-st7789-1.5.9/setup.py
```

### Comparing `adafruit-circuitpython-st7789-1.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-st7789-1.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/.github/workflows/build.yml` & `adafruit-circuitpython-st7789-1.5.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/.github/workflows/release.yml` & `adafruit-circuitpython-st7789-1.5.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/.gitignore` & `adafruit-circuitpython-st7789-1.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/.pre-commit-config.yaml` & `adafruit-circuitpython-st7789-1.5.9/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
+  - repo: https://github.com/python/black
     rev: 22.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v0.14.0
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.2.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
     rev: v2.11.1
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
-    -   id: pylint
+      - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
-        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-    -   id: pylint
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
         name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
         types: [python]
         files: "^tests/"
         args:
-        - --disable=missing-docstring,consider-using-f-string,duplicate-code
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-st7789-1.5.8/.pylintrc` & `adafruit-circuitpython-st7789-1.5.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-st7789-1.5.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-st7789-1.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/LICENSE` & `adafruit-circuitpython-st7789-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-st7789-1.5.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/LICENSES/MIT.txt` & `adafruit-circuitpython-st7789-1.5.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-st7789-1.5.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/PKG-INFO` & `adafruit-circuitpython-st7789-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-st7789
-Version: 1.5.8
+Version: 1.5.9
 Summary: displayio driver for ST7789 TFT-LCD displays.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_ST7789
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython st7789 display tft lcd displayio
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-st7789-1.5.8/README.rst` & `adafruit-circuitpython-st7789-1.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/adafruit_circuitpython_st7789.egg-info/PKG-INFO` & `adafruit-circuitpython-st7789-1.5.9/adafruit_circuitpython_st7789.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-st7789
-Version: 1.5.8
+Version: 1.5.9
 Summary: displayio driver for ST7789 TFT-LCD displays.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_ST7789
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython st7789 display tft lcd displayio
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-st7789-1.5.8/adafruit_circuitpython_st7789.egg-info/SOURCES.txt` & `adafruit-circuitpython-st7789-1.5.9/adafruit_circuitpython_st7789.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/adafruit_st7789.py` & `adafruit-circuitpython-st7789-1.5.9/adafruit_st7789.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/docs/_static/favicon.ico` & `adafruit-circuitpython-st7789-1.5.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/docs/conf.py` & `adafruit-circuitpython-st7789-1.5.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-st7789-1.5.8/docs/examples.rst` & `adafruit-circuitpython-st7789-1.5.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/docs/index.rst` & `adafruit-circuitpython-st7789-1.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_170x320_1.9_simpletest.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_170x320_1.9_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_172x320_1.47_simpletest.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_172x320_1.47_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x135_pitft_simpletest.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x135_pitft_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x135_simpletest.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x135_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x135_simpletest_Pimoroni_Pico_Display_Pack.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x135_simpletest_Pimoroni_Pico_Display_Pack.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x240_bonnet_simpletest.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x240_bonnet_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x240_pitft_simpletest.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x240_pitft_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x240_simpletest_Pimoroni_Pico_Explorer.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x240_simpletest_Pimoroni_Pico_Explorer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_240x240_simpletest_Waveshare_PicoLCD_1_3.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_240x240_simpletest_Waveshare_PicoLCD_1_3.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_280x240_simpletest.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_280x240_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_320x240_simpletest.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_320x240_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_320x240_simpletest_Pimoroni_Pico_Display_2_0.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_320x240_simpletest_Pimoroni_Pico_Display_2_0.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_simpletest.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/examples/st7789_tft_gizmo_simpletest.py` & `adafruit-circuitpython-st7789-1.5.9/examples/st7789_tft_gizmo_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-st7789-1.5.8/setup.py` & `adafruit-circuitpython-st7789-1.5.9/setup.py`

 * *Files identical despite different names*
