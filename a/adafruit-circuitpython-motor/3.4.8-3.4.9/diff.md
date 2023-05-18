# Comparing `tmp/adafruit-circuitpython-motor-3.4.8.tar.gz` & `tmp/adafruit-circuitpython-motor-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-motor-3.4.8.tar", last modified: Sat Feb  4 14:38:51 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-motor-3.4.9.tar", last modified: Tue Feb  7 23:18:26 2023, max compression
```

## Comparing `adafruit-circuitpython-motor-3.4.8.tar` & `adafruit-circuitpython-motor-3.4.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 14:38:51.783702 adafruit-circuitpython-motor-3.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 14:38:51.775702 adafruit-circuitpython-motor-3.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 14:38:51.779702 adafruit-circuitpython-motor-3.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 14:38:51.779702 adafruit-circuitpython-motor-3.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 14:38:51.779702 adafruit-circuitpython-motor-3.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-02-04 14:38:51.783702 adafruit-circuitpython-motor-3.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 14:38:51.779702 adafruit-circuitpython-motor-3.4.8/adafruit_circuitpython_motor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-02-04 14:38:51.000000 adafruit-circuitpython-motor-3.4.8/adafruit_circuitpython_motor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-02-04 14:38:51.000000 adafruit-circuitpython-motor-3.4.8/adafruit_circuitpython_motor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 14:38:51.000000 adafruit-circuitpython-motor-3.4.8/adafruit_circuitpython_motor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-04 14:38:51.000000 adafruit-circuitpython-motor-3.4.8/adafruit_circuitpython_motor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-04 14:38:51.000000 adafruit-circuitpython-motor-3.4.8/adafruit_circuitpython_motor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 14:38:51.779702 adafruit-circuitpython-motor-3.4.8/adafruit_motor/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/adafruit_motor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/adafruit_motor/motor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/adafruit_motor/servo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9953 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/adafruit_motor/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 14:38:51.783702 adafruit-circuitpython-motor-3.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 14:38:51.783702 adafruit-circuitpython-motor-3.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 14:38:51.783702 adafruit-circuitpython-motor-3.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/examples/motor_h-bridge_dc_motor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/examples/motor_pca9685_continuous_servo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/examples/motor_pca9685_dc_motor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/examples/motor_pca9685_servo_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/examples/motor_pca9685_stepper_motor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/examples/motor_servo_sweep_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1743 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/examples/motor_stepper_digitalio.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-04 14:38:35.000000 adafruit-circuitpython-motor-3.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 14:38:51.783702 adafruit-circuitpython-motor-3.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 14:38:51.783702 adafruit-circuitpython-motor-3.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-02-04 14:38:44.000000 adafruit-circuitpython-motor-3.4.8/tests/test_stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:18:26.448238 adafruit-circuitpython-motor-3.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:18:26.444237 adafruit-circuitpython-motor-3.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:18:26.444237 adafruit-circuitpython-motor-3.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:18:26.448238 adafruit-circuitpython-motor-3.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:18:26.448238 adafruit-circuitpython-motor-3.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-02-07 23:18:26.448238 adafruit-circuitpython-motor-3.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:18:26.448238 adafruit-circuitpython-motor-3.4.9/adafruit_circuitpython_motor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-02-07 23:18:26.000000 adafruit-circuitpython-motor-3.4.9/adafruit_circuitpython_motor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-02-07 23:18:26.000000 adafruit-circuitpython-motor-3.4.9/adafruit_circuitpython_motor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 23:18:26.000000 adafruit-circuitpython-motor-3.4.9/adafruit_circuitpython_motor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-07 23:18:26.000000 adafruit-circuitpython-motor-3.4.9/adafruit_circuitpython_motor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-07 23:18:26.000000 adafruit-circuitpython-motor-3.4.9/adafruit_circuitpython_motor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:18:26.448238 adafruit-circuitpython-motor-3.4.9/adafruit_motor/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/adafruit_motor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/adafruit_motor/motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/adafruit_motor/servo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9953 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/adafruit_motor/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:18:26.448238 adafruit-circuitpython-motor-3.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:18:26.448238 adafruit-circuitpython-motor-3.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:18:26.448238 adafruit-circuitpython-motor-3.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/examples/motor_h-bridge_dc_motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/examples/motor_pca9685_continuous_servo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/examples/motor_pca9685_dc_motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/examples/motor_pca9685_servo_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/examples/motor_pca9685_stepper_motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/examples/motor_servo_sweep_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1743 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/examples/motor_stepper_digitalio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-07 23:18:03.000000 adafruit-circuitpython-motor-3.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 23:18:26.448238 adafruit-circuitpython-motor-3.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:18:26.448238 adafruit-circuitpython-motor-3.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-02-07 23:18:18.000000 adafruit-circuitpython-motor-3.4.9/tests/test_stepper.py
```

### Comparing `adafruit-circuitpython-motor-3.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-motor-3.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/.gitignore` & `adafruit-circuitpython-motor-3.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-motor-3.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/.pylintrc` & `adafruit-circuitpython-motor-3.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-motor-3.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/LICENSE` & `adafruit-circuitpython-motor-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-motor-3.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-motor-3.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-motor-3.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/PKG-INFO` & `adafruit-circuitpython-motor-3.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-motor
-Version: 3.4.8
+Version: 3.4.9
 Summary: CircuitPython helper library provides higher level objects to control motors and servos.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Motor
 Keywords: adafruit,servo,stepper,motor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-motor-3.4.8/README.rst` & `adafruit-circuitpython-motor-3.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/adafruit_circuitpython_motor.egg-info/PKG-INFO` & `adafruit-circuitpython-motor-3.4.9/adafruit_circuitpython_motor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-motor
-Version: 3.4.8
+Version: 3.4.9
 Summary: CircuitPython helper library provides higher level objects to control motors and servos.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Motor
 Keywords: adafruit,servo,stepper,motor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-motor-3.4.8/adafruit_circuitpython_motor.egg-info/SOURCES.txt` & `adafruit-circuitpython-motor-3.4.9/adafruit_circuitpython_motor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/adafruit_motor/motor.py` & `adafruit-circuitpython-motor-3.4.9/adafruit_motor/motor.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         from pwmio import PWMOut
     except NotImplementedError:
         from circuitpython_typing.pwmio import PWMOut
 
 except ImportError:
     pass
 
-__version__ = "3.4.8"
+__version__ = "3.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Motor.git"
 
 FAST_DECAY = 0
 """Recirculation current fast decay mode (coasting)"""
 
 SLOW_DECAY = 1
 """Recirculation current slow decay mode (braking)"""
```

### Comparing `adafruit-circuitpython-motor-3.4.8/adafruit_motor/servo.py` & `adafruit-circuitpython-motor-3.4.9/adafruit_motor/servo.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     except NotImplementedError:
         from circuitpython_typing.pwmio import PWMOut
 
 except (ImportError, NotImplementedError):
     pass
 
 
-__version__ = "3.4.8"
+__version__ = "3.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Motor.git"
 
 # We disable the too few public methods check because this is a private base class for the two types
 # of servos.
 class _BaseServo:  # pylint: disable-msg=too-few-public-methods
     """Shared base class that handles pulse output based on a value between 0 and 1.0
```

### Comparing `adafruit-circuitpython-motor-3.4.8/adafruit_motor/stepper.py` & `adafruit-circuitpython-motor-3.4.9/adafruit_motor/stepper.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         from pwmio import PWMOut
     except NotImplementedError:
         from circuitpython_typing.pwmio import PWMOut
 
 except ImportError:
     pass
 
-__version__ = "3.4.8"
+__version__ = "3.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Motor.git"
 
 # Stepper Motor Shield/Wing Driver
 # Based on Adafruit Motorshield library:
 # https://github.com/adafruit/Adafruit_Motor_Shield_V2_Library
 
 # Constants that specify the direction and style of steps.
```

### Comparing `adafruit-circuitpython-motor-3.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-motor-3.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/docs/conf.py` & `adafruit-circuitpython-motor-3.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/docs/index.rst` & `adafruit-circuitpython-motor-3.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/examples/motor_h-bridge_dc_motor.py` & `adafruit-circuitpython-motor-3.4.9/examples/motor_h-bridge_dc_motor.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/examples/motor_pca9685_continuous_servo.py` & `adafruit-circuitpython-motor-3.4.9/examples/motor_pca9685_continuous_servo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/examples/motor_pca9685_dc_motor.py` & `adafruit-circuitpython-motor-3.4.9/examples/motor_pca9685_dc_motor.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/examples/motor_pca9685_servo_sweep.py` & `adafruit-circuitpython-motor-3.4.9/examples/motor_pca9685_servo_sweep.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/examples/motor_pca9685_stepper_motor.py` & `adafruit-circuitpython-motor-3.4.9/examples/motor_pca9685_stepper_motor.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/examples/motor_servo_sweep_simpletest.py` & `adafruit-circuitpython-motor-3.4.9/examples/motor_servo_sweep_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/examples/motor_stepper_digitalio.py` & `adafruit-circuitpython-motor-3.4.9/examples/motor_stepper_digitalio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motor-3.4.8/pyproject.toml` & `adafruit-circuitpython-motor-3.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-motor"
 description = "CircuitPython helper library provides higher level objects to control motors and servos."
-version = "3.4.8"
+version = "3.4.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Motor"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-motor-3.4.8/tests/test_stepper.py` & `adafruit-circuitpython-motor-3.4.9/tests/test_stepper.py`

 * *Files identical despite different names*

