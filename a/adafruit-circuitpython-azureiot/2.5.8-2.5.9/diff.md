# Comparing `tmp/adafruit-circuitpython-azureiot-2.5.8.tar.gz` & `tmp/adafruit-circuitpython-azureiot-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-azureiot-2.5.8.tar", last modified: Wed Jul 27 19:54:01 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-azureiot-2.5.9.tar", last modified: Tue Aug  9 19:32:49 2022, max compression
```

## Comparing `adafruit-circuitpython-azureiot-2.5.8.tar` & `adafruit-circuitpython-azureiot-2.5.9.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.259307 adafruit-circuitpython-azureiot-2.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.247306 adafruit-circuitpython-azureiot-2.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.251306 adafruit-circuitpython-azureiot-2.5.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.251306 adafruit-circuitpython-azureiot-2.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16261 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.251306 adafruit-circuitpython-azureiot-2.5.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12352 2022-07-27 19:54:01.259307 adafruit-circuitpython-azureiot-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11599 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.255306 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/base64.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/device_registration.py
--rw-r--r--   0 runner    (1001) docker     (121)    17792 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/hmac.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/iot_error.py
--rw-r--r--   0 runner    (1001) docker     (121)    17202 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/iot_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (121)     8889 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/iotcentral_device.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15024 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/iothub_device.py
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     3921 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/quote.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.255306 adafruit-circuitpython-azureiot-2.5.8/adafruit_circuitpython_azureiot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12352 2022-07-27 19:54:01.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_circuitpython_azureiot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2733 2022-07-27 19:54:01.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_circuitpython_azureiot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-27 19:54:01.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_circuitpython_azureiot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-07-27 19:54:01.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_circuitpython_azureiot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-27 19:54:01.000000 adafruit-circuitpython-azureiot-2.5.8/adafruit_circuitpython_azureiot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.255306 adafruit-circuitpython-azureiot-2.5.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.255306 adafruit-circuitpython-azureiot-2.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5570 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3911 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    19120 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/iot-central-connect-button.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/iot-central-connect-button.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    74478 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/iot-central-connect-dialog.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/iot-central-connect-dialog.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    72070 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/iot-hub-device-keys.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/iot-hub-device-keys.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    70638 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/iot-hub-device.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/iot-hub-device.png.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.255306 adafruit-circuitpython-azureiot-2.5.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.259307 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/
--rw-r--r--   0 runner    (1001) docker     (121)     5083 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_central_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     3931 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_central_notconnected.py
--rw-r--r--   0 runner    (1001) docker     (121)     5092 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_central_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     4707 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_central_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4765 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_hub_directmethods.py
--rw-r--r--   0 runner    (1001) docker     (121)     4881 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_hub_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     4371 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_hub_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5198 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_hub_twin_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-27 19:54:01.259307 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_central_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     2948 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_central_notconnected.py
--rw-r--r--   0 runner    (1001) docker     (121)     3922 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_central_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_central_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_hub_directmethods.py
--rw-r--r--   0 runner    (1001) docker     (121)     3865 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_hub_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     3381 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_hub_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4076 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_hub_twin_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_secrets_example.py
--rw-r--r--   0 runner    (1001) docker     (121)    19120 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/iot-central-connect-button.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/iot-central-connect-button.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    74478 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/iot-central-connect-dialog.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/iot-central-connect-dialog.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    72070 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/iot-hub-device-keys.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/iot-hub-device-keys.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    70638 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/iot-hub-device.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/iot-hub-device.png.license
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-27 19:54:01.259307 adafruit-circuitpython-azureiot-2.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-07-27 19:53:43.000000 adafruit-circuitpython-azureiot-2.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.009276 adafruit-circuitpython-azureiot-2.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.985276 adafruit-circuitpython-azureiot-2.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.989276 adafruit-circuitpython-azureiot-2.5.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.989276 adafruit-circuitpython-azureiot-2.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16261 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.993276 adafruit-circuitpython-azureiot-2.5.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12524 2022-08-09 19:32:49.009276 adafruit-circuitpython-azureiot-2.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11740 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.993276 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/
+-rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/base64.py
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/device_registration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17792 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iot_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17202 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iot_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8889 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iotcentral_device.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    15024 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iothub_device.py
+-rw-r--r--   0 runner    (1001) docker     (121)      776 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3921 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.997276 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12524 2022-08-09 19:32:48.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2765 2022-08-09 19:32:48.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:32:48.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-08-09 19:32:48.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-09 19:32:48.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.001276 adafruit-circuitpython-azureiot-2.5.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.001276 adafruit-circuitpython-azureiot-2.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5570 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3911 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)    19120 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-button.png
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-button.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)    74478 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-dialog.png
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-dialog.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)    72070 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device-keys.png
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device-keys.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)    70638 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device.png
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.001276 adafruit-circuitpython-azureiot-2.5.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.005276 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (121)     5083 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3931 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_notconnected.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5092 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4707 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4765 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_directmethods.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4881 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_messages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4371 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5198 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_twin_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.009276 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/
+-rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2948 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_notconnected.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3922 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_directmethods.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3865 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_messages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3381 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4076 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_twin_operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_secrets_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19120 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-button.png
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-button.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)    74478 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-dialog.png
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-dialog.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)    72070 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-hub-device-keys.png
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-hub-device-keys.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)    70638 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-hub-device.png
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-hub-device.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:32:49.009276 adafruit-circuitpython-azureiot-2.5.9/setup.cfg
```

### Comparing `adafruit-circuitpython-azureiot-2.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-azureiot-2.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/.github/workflows/build.yml` & `adafruit-circuitpython-azureiot-2.5.9/.github/workflows/build.yml`

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

### Comparing `adafruit-circuitpython-azureiot-2.5.8/.gitignore` & `adafruit-circuitpython-azureiot-2.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/.pre-commit-config.yaml` & `adafruit-circuitpython-azureiot-2.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/.pylintrc` & `adafruit-circuitpython-azureiot-2.5.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-azureiot-2.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/LICENSE` & `adafruit-circuitpython-azureiot-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-azureiot-2.5.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/LICENSES/MIT.txt` & `adafruit-circuitpython-azureiot-2.5.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-azureiot-2.5.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/PKG-INFO` & `adafruit-circuitpython-azureiot-2.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-azureiot
-Version: 2.5.8
+Version: 2.5.9
 Summary: Access to Microsoft Azure IoT from CircuitPython
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython azureiot azure iot device services,iothub,iotcentral
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT
+Keywords: adafruit,blinka,circuitpython,micropython,azureiot,azure,iot,device,services,,iothub,,iotcentral
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Adafruit_CircuitPython_AzureIoT
 ================================
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-azureiot/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/azureiot/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 A CircuitPython device library for `Microsoft Azure IoT Services <https://azure.microsoft.com/overview/iot/?WT.mc_id=academic-3168-jabenn>`_ from a CircuitPython device. This library only supports key-base authentication, it currently doesn't support X.509 certificates.
 
 Installing from PyPI
 =====================
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/adafruit-circuitpython-azureiot/>`_. To install for current user:
 
@@ -304,9 +307,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-azureiot-2.5.8/README.rst` & `adafruit-circuitpython-azureiot-2.5.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 A CircuitPython device library for `Microsoft Azure IoT Services <https://azure.microsoft.com/overview/iot/?WT.mc_id=academic-3168-jabenn>`_ from a CircuitPython device. This library only supports key-base authentication, it currently doesn't support X.509 certificates.
 
 Installing from PyPI
 =====================
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/adafruit-circuitpython-azureiot/>`_. To install for current user:
```

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/__init__.py` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,11 +32,11 @@
 """
 
 from .iot_error import IoTError
 from .iot_mqtt import IoTResponse
 from .iotcentral_device import IoTCentralDevice
 from .iothub_device import IoTHubDevice
 
-__version__ = "0.0.0-auto.0"
+__version__ = "2.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT.git"
 
 __all__ = ["IoTHubDevice", "IoTCentralDevice", "IoTResponse", "IoTError"]
```

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/base64.py` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/base64.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/constants.py` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/constants.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/device_registration.py` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/device_registration.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/hmac.py` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/hmac.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/iot_error.py` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iot_error.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/iot_mqtt.py` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iot_mqtt.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/iotcentral_device.py` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iotcentral_device.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/iothub_device.py` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iothub_device.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/keys.py` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/keys.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_azureiot/quote.py` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/quote.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_circuitpython_azureiot.egg-info/PKG-INFO` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-azureiot
-Version: 2.5.8
+Version: 2.5.9
 Summary: Access to Microsoft Azure IoT from CircuitPython
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython azureiot azure iot device services,iothub,iotcentral
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT
+Keywords: adafruit,blinka,circuitpython,micropython,azureiot,azure,iot,device,services,,iothub,,iotcentral
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Adafruit_CircuitPython_AzureIoT
 ================================
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-azureiot/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/azureiot/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 A CircuitPython device library for `Microsoft Azure IoT Services <https://azure.microsoft.com/overview/iot/?WT.mc_id=academic-3168-jabenn>`_ from a CircuitPython device. This library only supports key-base authentication, it currently doesn't support X.509 certificates.
 
 Installing from PyPI
 =====================
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/adafruit-circuitpython-azureiot/>`_. To install for current user:
 
@@ -304,9 +307,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-azureiot-2.5.8/adafruit_circuitpython_azureiot.egg-info/SOURCES.txt` & `adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 iot-central-connect-button.png.license
 iot-central-connect-dialog.png
 iot-central-connect-dialog.png.license
 iot-hub-device-keys.png
 iot-hub-device-keys.png.license
 iot-hub-device.png
 iot-hub-device.png.license
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
```

### Comparing `adafruit-circuitpython-azureiot-2.5.8/docs/_static/favicon.ico` & `adafruit-circuitpython-azureiot-2.5.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/docs/conf.py` & `adafruit-circuitpython-azureiot-2.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/docs/examples.rst` & `adafruit-circuitpython-azureiot-2.5.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/docs/index.rst` & `adafruit-circuitpython-azureiot-2.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/docs/iot-central-connect-button.png` & `adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-button.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/docs/iot-central-connect-dialog.png` & `adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-dialog.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/docs/iot-hub-device-keys.png` & `adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device-keys.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/docs/iot-hub-device.png` & `adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_central_commands.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_commands.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_central_notconnected.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_notconnected.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_central_properties.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_properties.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_central_simpletest.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_hub_directmethods.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_directmethods.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_hub_messages.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_messages.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_hub_simpletest.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_esp32spi/azureiot_hub_twin_operations.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_twin_operations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_central_commands.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_commands.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_central_notconnected.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_notconnected.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_central_properties.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_properties.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_central_simpletest.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_hub_directmethods.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_directmethods.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_hub_messages.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_messages.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_hub_simpletest.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_native_networking/azureiot_hub_twin_operations.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_twin_operations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/examples/azureiot_secrets_example.py` & `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_secrets_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/iot-central-connect-button.png` & `adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-button.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/iot-central-connect-dialog.png` & `adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-dialog.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/iot-hub-device-keys.png` & `adafruit-circuitpython-azureiot-2.5.9/iot-hub-device-keys.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.8/iot-hub-device.png` & `adafruit-circuitpython-azureiot-2.5.9/iot-hub-device.png`

 * *Files identical despite different names*

