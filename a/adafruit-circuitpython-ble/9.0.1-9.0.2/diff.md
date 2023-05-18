# Comparing `tmp/adafruit-circuitpython-ble-9.0.1.tar.gz` & `tmp/adafruit-circuitpython-ble-9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-9.0.1.tar", last modified: Tue Nov 15 18:27:30 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-9.0.2.tar", last modified: Mon Mar 13 16:51:52 2023, max compression
```

## Comparing `adafruit-circuitpython-ble-9.0.1.tar` & `adafruit-circuitpython-ble-9.0.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.786422 adafruit-circuitpython-ble-9.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.770422 adafruit-circuitpython-ble-9.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.774422 adafruit-circuitpython-ble-9.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.774422 adafruit-circuitpython-ble-9.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.774422 adafruit-circuitpython-ble-9.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3678 2022-11-15 18:27:30.786422 adafruit-circuitpython-ble-9.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2941 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.774422 adafruit-circuitpython-ble-9.0.1/adafruit_ble/
--rwxr-xr-x   0 runner    (1001) docker     (122)    13927 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.774422 adafruit-circuitpython-ble-9.0.1/adafruit_ble/advertising/
--rw-r--r--   0 runner    (1001) docker     (122)    12930 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/advertising/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1612 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/advertising/adafruit.py
--rw-r--r--   0 runner    (1001) docker     (122)    17006 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/advertising/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.774422 adafruit-circuitpython-ble-9.0.1/adafruit_ble/attributes/
--rw-r--r--   0 runner    (1001) docker     (122)     1639 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/attributes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.778422 adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/
--rw-r--r--   0 runner    (1001) docker     (122)    10091 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/float.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3829 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/int.py
--rw-r--r--   0 runner    (1001) docker     (122)     2095 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/json.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3712 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/stream.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2341 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/string.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.778422 adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/
--rw-r--r--   0 runner    (1001) docker     (122)     3240 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1265 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/circuitpython.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/microbit.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3256 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/nordic.py
--rw-r--r--   0 runner    (1001) docker     (122)      512 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/sphero.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.778422 adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/standard/
--rw-r--r--   0 runner    (1001) docker     (122)     2556 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2571 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/standard/device_info.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    16903 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/standard/hid.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.778422 adafruit-circuitpython-ble-9.0.1/adafruit_ble/uuid/
--rw-r--r--   0 runner    (1001) docker     (122)     1608 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/adafruit_ble/uuid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.778422 adafruit-circuitpython-ble-9.0.1/adafruit_circuitpython_ble.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3678 2022-11-15 18:27:30.000000 adafruit-circuitpython-ble-9.0.1/adafruit_circuitpython_ble.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2579 2022-11-15 18:27:30.000000 adafruit-circuitpython-ble-9.0.1/adafruit_circuitpython_ble.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-15 18:27:30.000000 adafruit-circuitpython-ble-9.0.1/adafruit_circuitpython_ble.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-11-15 18:27:30.000000 adafruit-circuitpython-ble-9.0.1/adafruit_circuitpython_ble.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2022-11-15 18:27:30.000000 adafruit-circuitpython-ble-9.0.1/adafruit_circuitpython_ble.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.782422 adafruit-circuitpython-ble-9.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.782422 adafruit-circuitpython-ble-9.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      272 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/advertising.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/advertising.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      186 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      142 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/attributes.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/attributes.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      399 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/characteristics.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/characteristics.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5708 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      450 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      347 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/services.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/services.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      294 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/standard_services.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/standard_services.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      130 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/uuid.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/docs/uuid.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:27:30.786422 adafruit-circuitpython-ble-9.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      595 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_advertising_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1023 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_bluefruit_color_picker.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1151 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_bluefruit_connect_plotter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3418 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_color_proximity.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_current_time_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     2316 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_demo_central.py
--rw-r--r--   0 runner    (1001) docker     (122)     1293 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_demo_periph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_detailed_scan.py
--rw-r--r--   0 runner    (1001) docker     (122)     1036 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_device_info_service.py
--rw-r--r--   0 runner    (1001) docker     (122)      790 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_hid_central.py
--rw-r--r--   0 runner    (1001) docker     (122)     1360 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_hid_periph.py
--rw-r--r--   0 runner    (1001) docker     (122)      934 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_json_central.py
--rw-r--r--   0 runner    (1001) docker     (122)     1518 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_json_peripheral.py
--rw-r--r--   0 runner    (1001) docker     (122)     1406 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_json_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     1284 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_packet_buffer_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_packet_buffer_service.py
--rw-r--r--   0 runner    (1001) docker     (122)      828 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_packet_buffer_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      721 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1195 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_uart_echo_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      802 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/examples/ble_uart_echo_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2022-11-15 18:27:22.000000 adafruit-circuitpython-ble-9.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      207 2022-11-15 18:27:13.000000 adafruit-circuitpython-ble-9.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-15 18:27:30.786422 adafruit-circuitpython-ble-9.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.884812 adafruit-circuitpython-ble-9.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.872812 adafruit-circuitpython-ble-9.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.876812 adafruit-circuitpython-ble-9.0.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.876812 adafruit-circuitpython-ble-9.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.876812 adafruit-circuitpython-ble-9.0.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-03-13 16:51:52.884812 adafruit-circuitpython-ble-9.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.876812 adafruit-circuitpython-ble-9.0.2/adafruit_ble/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13951 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.876812 adafruit-circuitpython-ble-9.0.2/adafruit_ble/advertising/
+-rw-r--r--   0 runner    (1001) docker     (123)    12930 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/advertising/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1612 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/advertising/adafruit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/advertising/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.876812 adafruit-circuitpython-ble-9.0.2/adafruit_ble/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/attributes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.876812 adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/float.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3829 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3712 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2341 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.880812 adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1265 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/circuitpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/microbit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3256 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/nordic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/sphero.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.880812 adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/standard/device_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16903 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/standard/hid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.880812 adafruit-circuitpython-ble-9.0.2/adafruit_ble/uuid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/adafruit_ble/uuid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.880812 adafruit-circuitpython-ble-9.0.2/adafruit_circuitpython_ble.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-03-13 16:51:52.000000 adafruit-circuitpython-ble-9.0.2/adafruit_circuitpython_ble.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-03-13 16:51:52.000000 adafruit-circuitpython-ble-9.0.2/adafruit_circuitpython_ble.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 16:51:52.000000 adafruit-circuitpython-ble-9.0.2/adafruit_circuitpython_ble.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-13 16:51:52.000000 adafruit-circuitpython-ble-9.0.2/adafruit_circuitpython_ble.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-13 16:51:52.000000 adafruit-circuitpython-ble-9.0.2/adafruit_circuitpython_ble.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.880812 adafruit-circuitpython-ble-9.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.880812 adafruit-circuitpython-ble-9.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/advertising.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/advertising.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/attributes.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/characteristics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/characteristics.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/services.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/standard_services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/standard_services.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/uuid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/docs/uuid.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 16:51:52.884812 adafruit-circuitpython-ble-9.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_advertising_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_bluefruit_color_picker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1151 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_bluefruit_connect_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_color_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_current_time_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_demo_central.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_demo_periph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_detailed_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_device_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_hid_central.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_hid_periph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_json_central.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_json_peripheral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_json_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_packet_buffer_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_packet_buffer_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_packet_buffer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_uart_echo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/examples/ble_uart_echo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-13 16:51:45.000000 adafruit-circuitpython-ble-9.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-13 16:51:37.000000 adafruit-circuitpython-ble-9.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 16:51:52.884812 adafruit-circuitpython-ble-9.0.2/setup.cfg
```

### Comparing `adafruit-circuitpython-ble-9.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-9.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/.gitignore` & `adafruit-circuitpython-ble-9.0.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-ble-9.0.1/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-9.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/.pylintrc` & `adafruit-circuitpython-ble-9.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-9.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/LICENSE` & `adafruit-circuitpython-ble-9.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-9.0.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-9.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-9.0.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/PKG-INFO` & `adafruit-circuitpython-ble-9.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble
-Version: 9.0.1
+Version: 9.0.2
 Summary: Bluetooth Low Energy (BLE) library for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE
 Keywords: adafruit,blinka,circuitpython,micropython,ble,bluetooth
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-9.0.1/README.rst` & `adafruit-circuitpython-ble-9.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/__init__.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,26 +24,26 @@
 
 import _bleio
 
 from .services import Service
 from .advertising import Advertisement
 
 try:
-    from typing import Optional, Iterator, Union, Tuple, NoReturn, TYPE_CHECKING
+    from typing import Iterator, NoReturn, Optional, Tuple, Type, TYPE_CHECKING, Union
     from typing_extensions import Literal
 
     if TYPE_CHECKING:
         from circuitpython_typing import ReadableBuffer
         from adafruit_ble.uuid import UUID
         from adafruit_ble.characteristics import Characteristic
 
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class BLEConnection:
     """
     Represents a connection to a peer BLE device.
     It acts as a map from a `Service` type to a `Service` instance for the connection.
@@ -68,15 +68,15 @@
                 (uuid.bleio_uuid,)
             )
             if results:
                 remote_service = results[0]
                 self._discovered_bleio_services[uuid] = remote_service
         return remote_service
 
-    def __contains__(self, key: Union[UUID, Service]) -> bool:
+    def __contains__(self, key: Union[UUID, Type[Service]]) -> bool:
         """
         Allows easy testing for a particular Service class or a particular UUID
         associated with this connection.
 
         Example::
 
             if UARTService in connection:
@@ -86,15 +86,15 @@
                 # do something
         """
         uuid = key
         if hasattr(key, "uuid"):
             uuid = key.uuid
         return self._discover_remote(uuid) is not None
 
-    def __getitem__(self, key: Union[UUID, Service]) -> Optional[Service]:
+    def __getitem__(self, key: Union[UUID, Type[Service]]) -> Optional[Service]:
         """Return the Service for the given Service class or uuid, if any."""
         uuid = key
         maybe_service = False
         if hasattr(key, "uuid"):
             uuid = key.uuid
             maybe_service = True
 
@@ -217,15 +217,15 @@
 
     def stop_advertising(self) -> None:
         """Stops advertising."""
         self._adapter.stop_advertising()
 
     def start_scan(
         self,
-        *advertisement_types: Advertisement,
+        *advertisement_types: Type[Advertisement],
         buffer_size: int = 512,
         extended: bool = False,
         timeout: Optional[float] = None,
         interval: float = 0.1,
         window: float = 0.1,
         minimum_rssi: int = -80,
         active: bool = True,
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/advertising/__init__.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/advertising/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/advertising/adafruit.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/advertising/adafruit.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import struct
 from micropython import const
 
 from . import Advertisement, LazyObjectField
 from .standard import ManufacturerData, ManufacturerDataField
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 MANUFACTURING_DATA_ADT = const(0xFF)
 """The advertising data type for manufacturer-specific data"""
 
 ADAFRUIT_COMPANY_ID = const(0x0822)
 """Company Identifier for Adafruit Industries"""
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/advertising/standard.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/advertising/standard.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         "ProvideServicesAdvertisement", "SolicitServicesAdvertisement"
     ]
 
 
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class BoundServiceList:
     """Sequence-like object of Service UUID objects. It stores both standard and vendor UUIDs."""
 
     def __init__(
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/attributes/__init__.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/attributes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 This module provides definitions common to all kinds of BLE attributes,
 specifically characteristics and descriptors.
 
 """
 import _bleio
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class Attribute:
     """Constants describing security levels.
 
     .. data:: NO_ACCESS
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/__init__.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         from circuitpython_typing import ReadableBuffer
         from adafruit_ble.uuid import UUID
         from adafruit_ble.services import Service
 
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class Characteristic:
     """
     Top level Characteristic class that does basic binding.
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/float.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/float.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         from circuitpython_typing import ReadableBuffer
         from adafruit_ble.uuid import UUID
         from adafruit_ble.services import Service
 
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class FloatCharacteristic(StructCharacteristic):
     """32-bit float"""
 
     def __init__(
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/int.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/int.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         from circuitpython_typing import ReadableBuffer
         from adafruit_ble.uuid import UUID
         from adafruit_ble.services import Service
 
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class IntCharacteristic(StructCharacteristic):
     """Superclass for different kinds of integer fields."""
 
     def __init__(
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/json.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         from circuitpython_typing import ReadableBuffer
         from adafruit_ble.uuid import UUID
         from adafruit_ble.services import Service
 
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class JSONCharacteristic(Characteristic):
     """JSON string characteristic for JSON serializable values of a limited size (max_length)."""
 
     def __init__(
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/stream.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         from adafruit_ble.characteristics import Characteristic
         from adafruit_ble.uuid import UUID
         from adafruit_ble.services import Service
 
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class BoundWriteStream:
     """Writes data out to the peer."""
 
     def __init__(self, bound_characteristic: Characteristic) -> None:
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/characteristics/string.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/characteristics/string.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         from circuitpython_typing import ReadableBuffer
         from adafruit_ble.uuid import UUID
         from adafruit_ble.services import Service
 
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class StringCharacteristic(Characteristic):
     """UTF-8 Encoded string characteristic."""
 
     def __init__(
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/__init__.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from ..characteristics import Characteristic, ComplexCharacteristic
 
 try:
     from typing import Optional
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class Service:
     """Top level Service class that handles the hard work of binding to a local or remote service.
 
     Providers of a local service should instantiate their Service with service=None, the default.
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/circuitpython.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/circuitpython.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from . import Service
 from ..characteristics import Characteristic
 from ..characteristics.stream import StreamOut
 from ..characteristics.string import StringCharacteristic
 from ..uuid import VendorUUID
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class CircuitPythonUUID(VendorUUID):
     """UUIDs with the CircuitPython base UUID."""
 
     def __init__(self, uuid16: int) -> None:
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/nordic.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/nordic.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     if TYPE_CHECKING:
         from circuitpython_typing import WriteableBuffer, ReadableBuffer
         import _bleio
 
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class UARTService(Service):
     """
     Provide UART-like functionality via the Nordic NUS service.
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/sphero.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/sphero.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 This module provides Services used by Sphero robots.
 
 """
 
 from . import Service
 from ..uuid import VendorUUID
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class SpheroService(Service):
     """Core Sphero Service. Unimplemented."""
 
     uuid = VendorUUID(b"!!orehpS OOW\x01\x00\x01\x00")
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/standard/__init__.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/standard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .. import Service
 from ...uuid import StandardUUID
 from ...characteristics import Characteristic
 from ...characteristics.string import StringCharacteristic
 from ...characteristics import StructCharacteristic
 from ...characteristics.int import Uint8Characteristic
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class AppearanceCharacteristic(StructCharacteristic):
     """What type of device it is"""
 
     # pylint: disable=too-few-public-methods
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/standard/device_info.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/standard/device_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     if TYPE_CHECKING:
         import _bleio
 
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class DeviceInfoService(Service):
     """Device information"""
 
     uuid = StandardUUID(0x180A)
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/services/standard/hid.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/services/standard/hid.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from .. import Service
 
 try:
     from typing import Dict, Optional
 except ImportError:
     pass
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 _HID_SERVICE_UUID_NUM = const(0x1812)
 _REPORT_UUID_NUM = const(0x2A4D)
 _REPORT_MAP_UUID_NUM = const(0x2A4B)
 _HID_INFORMATION_UUID_NUM = const(0x2A4A)
 _HID_CONTROL_POINT_UUID_NUM = const(0x2A4C)
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_ble/uuid/__init__.py` & `adafruit-circuitpython-ble-9.0.2/adafruit_ble/uuid/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 
 import struct
 
 import _bleio
 
-__version__ = "9.0.1"
+__version__ = "9.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE.git"
 
 
 class UUID:
     """Top level UUID"""
 
     # TODO: Make subclassing _bleio.UUID work so we can just use it directly.
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_circuitpython_ble.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-9.0.2/adafruit_circuitpython_ble.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble
-Version: 9.0.1
+Version: 9.0.2
 Summary: Bluetooth Low Energy (BLE) library for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE
 Keywords: adafruit,blinka,circuitpython,micropython,ble,bluetooth
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-9.0.1/adafruit_circuitpython_ble.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-9.0.2/adafruit_circuitpython_ble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-9.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/docs/conf.py` & `adafruit-circuitpython-ble-9.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/docs/index.rst` & `adafruit-circuitpython-ble-9.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_advertising_simpletest.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_advertising_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_bluefruit_color_picker.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_bluefruit_color_picker.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_bluefruit_connect_plotter.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_bluefruit_connect_plotter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_color_proximity.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_color_proximity.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_current_time_service.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_current_time_service.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_demo_central.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_demo_central.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_demo_periph.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_demo_periph.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_detailed_scan.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_detailed_scan.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_device_info_service.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_device_info_service.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_hid_central.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_hid_central.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_hid_periph.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_hid_periph.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_json_central.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_json_central.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_json_peripheral.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_json_peripheral.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_json_service.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_json_service.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_packet_buffer_client.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_packet_buffer_client.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_packet_buffer_service.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_packet_buffer_service.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_packet_buffer_test.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_packet_buffer_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_simpletest.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_uart_echo_client.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_uart_echo_client.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/examples/ble_uart_echo_test.py` & `adafruit-circuitpython-ble-9.0.2/examples/ble_uart_echo_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-9.0.1/pyproject.toml` & `adafruit-circuitpython-ble-9.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ble"
 description = "Bluetooth Low Energy (BLE) library for CircuitPython"
-version = "9.0.1"
+version = "9.0.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BLE"}
 keywords = [
     "adafruit",
```

