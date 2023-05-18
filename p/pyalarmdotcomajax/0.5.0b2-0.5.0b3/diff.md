# Comparing `tmp/pyalarmdotcomajax-0.5.0b2.tar.gz` & `tmp/pyalarmdotcomajax-0.5.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalarmdotcomajax-0.5.0b2.tar", last modified: Mon May 15 19:49:39 2023, max compression
+gzip compressed data, was "pyalarmdotcomajax-0.5.0b3.tar", last modified: Thu May 18 17:22:36 2023, max compression
```

## Comparing `pyalarmdotcomajax-0.5.0b2.tar` & `pyalarmdotcomajax-0.5.0b3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:49:39.904657 pyalarmdotcomajax-0.5.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-05-15 19:49:39.904657 pyalarmdotcomajax-0.5.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:49:39.900657 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/
--rw-r--r--   0 runner    (1001) docker     (123)    41855 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:49:39.900657 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/image_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:49:39.904657 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:49:39.904657 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:49:39.900657 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-05-15 19:49:39.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-15 19:49:39.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:49:39.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 19:49:39.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-15 19:49:39.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 19:49:39.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:49:39.000000 pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-15 19:49:39.904657 pyalarmdotcomajax-0.5.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:49:39.904657 pyalarmdotcomajax-0.5.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:49:39.904657 pyalarmdotcomajax-0.5.0b2/tests/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/tests/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/tests/test_device_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-15 19:49:28.000000 pyalarmdotcomajax-0.5.0b2/tests/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.590360 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/
+-rw-r--r--   0 runner    (1001) docker     (123)    40766 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/image_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.590360 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 17:22:36.598361 pyalarmdotcomajax-0.5.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/tests/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/test_device_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/test_thermostat.py
```

### Comparing `pyalarmdotcomajax-0.5.0b2/LICENSE` & `pyalarmdotcomajax-0.5.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/PKG-INFO` & `pyalarmdotcomajax-0.5.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.0b2
+Version: 0.5.0b3
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
@@ -67,17 +67,17 @@
 
 - As of v0.2, multiples of all devices are supported.
 - All devices include the attributes: `name`, `id_`, `state`, `battery_low`, `battery_critical`, `malfunctioning`, `parent_ids`, and a few others.
 
 | Device Type  | Notable Attributes                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Actions                               | Notes                                            |
 | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- | ------------------------------------------------ |
 | System       | `unit_id`                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | (none)                                |                                                  |
-| Partition    | `uncleared_issues`, `desired_state`                                                                                                                                                                                                                                                                                                                                                                                                                                       | arm away, arm stay, arm night, disarm |                                                  |
+| Partition    | `uncleared_issues`                                                                                                                                                                                                                                                                                                                                                                                                                                     | arm away, arm stay, arm night, disarm |                                                  |
 | Sensor       | `device_subtype`                                                                                                                                                                                                                                                                                                                                                                                                                                                          | (none)                                |                                                  |
-| Locks        | `desired_state`                                                                                                                                                                                                                                                                                                                                                                                                                                                           | lock, unlock                          |                                                  |
+| Locks        |                                                                                                                                                                                                                                                                                                                                                                                                                                                         | lock, unlock                          |                                                  |
 | Garage Door  | (none)                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | open, close                           |                                                  |
 | Gate         | `supports_remote_close`                                                                                                                                                                                                                                                                                                                                                                                                                                                   | open, close                           |                                                  |
 | Image Sensor | `images`                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | peek_in                               |                                                  |
 | Light        | `brightness`                                                                                                                                                                                                                                                                                                                                                                                                                                                              | turn_on (with brightness), turn_off   | No support for RGB/W, effects, temperature, etc. |
 | Thermostat   | `temp_average`, `temp_at_tstat`, `step_value`, `supports_fan_mode`, `supports_fan_indefinite`, `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`, `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`, `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`, `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`, `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` | set_attribute                         |                                                  |
 | Water Sensor |                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | (none)                                |                                                  |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b2 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b3 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
@@ -36,22 +36,21 @@
 ---- | ------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------------------------- | -------
 ------------------------------ | ----------------------------------------------
--- | | System | `unit_id` | (none) | | | Partition | `uncleared_issues`,
-`desired_state` | arm away, arm stay, arm night, disarm | | | Sensor |
-`device_subtype` | (none) | | | Locks | `desired_state` | lock, unlock | | |
-Garage Door | (none) | open, close | | | Gate | `supports_remote_close` | open,
-close | | | Image Sensor | `images` | peek_in | | | Light | `brightness` |
-turn_on (with brightness), turn_off | No support for RGB/W, effects,
-temperature, etc. | | Thermostat | `temp_average`, `temp_at_tstat`,
-`step_value`, `supports_fan_mode`, `supports_fan_indefinite`,
+-- | | System | `unit_id` | (none) | | | Partition | `uncleared_issues` | arm
+away, arm stay, arm night, disarm | | | Sensor | `device_subtype` | (none) | |
+| Locks | | lock, unlock | | | Garage Door | (none) | open, close | | | Gate |
+`supports_remote_close` | open, close | | | Image Sensor | `images` | peek_in |
+| | Light | `brightness` | turn_on (with brightness), turn_off | No support for
+RGB/W, effects, temperature, etc. | | Thermostat | `temp_average`,
+`temp_at_tstat`, `step_value`, `supports_fan_mode`, `supports_fan_indefinite`,
 `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`,
 `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`,
 `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`,
 `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`,
 `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` |
 set_attribute | | | Water Sensor | | (none) | | ### Known Sensor deviceTypes
 This list identifies deviceTypes used in the alarm.com API and is incomplete.
```

### Comparing `pyalarmdotcomajax-0.5.0b2/README.md` & `pyalarmdotcomajax-0.5.0b3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
 - As of v0.2, multiples of all devices are supported.
 - All devices include the attributes: `name`, `id_`, `state`, `battery_low`, `battery_critical`, `malfunctioning`, `parent_ids`, and a few others.
 
 | Device Type  | Notable Attributes                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Actions                               | Notes                                            |
 | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- | ------------------------------------------------ |
 | System       | `unit_id`                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | (none)                                |                                                  |
-| Partition    | `uncleared_issues`, `desired_state`                                                                                                                                                                                                                                                                                                                                                                                                                                       | arm away, arm stay, arm night, disarm |                                                  |
+| Partition    | `uncleared_issues`                                                                                                                                                                                                                                                                                                                                                                                                                                     | arm away, arm stay, arm night, disarm |                                                  |
 | Sensor       | `device_subtype`                                                                                                                                                                                                                                                                                                                                                                                                                                                          | (none)                                |                                                  |
-| Locks        | `desired_state`                                                                                                                                                                                                                                                                                                                                                                                                                                                           | lock, unlock                          |                                                  |
+| Locks        |                                                                                                                                                                                                                                                                                                                                                                                                                                                         | lock, unlock                          |                                                  |
 | Garage Door  | (none)                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | open, close                           |                                                  |
 | Gate         | `supports_remote_close`                                                                                                                                                                                                                                                                                                                                                                                                                                                   | open, close                           |                                                  |
 | Image Sensor | `images`                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | peek_in                               |                                                  |
 | Light        | `brightness`                                                                                                                                                                                                                                                                                                                                                                                                                                                              | turn_on (with brightness), turn_off   | No support for RGB/W, effects, temperature, etc. |
 | Thermostat   | `temp_average`, `temp_at_tstat`, `step_value`, `supports_fan_mode`, `supports_fan_indefinite`, `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`, `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`, `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`, `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`, `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` | set_attribute                         |                                                  |
 | Water Sensor |                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | (none)                                |                                                  |
```

#### html2text {}

```diff
@@ -22,22 +22,21 @@
 ---- | ------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------------------------- | -------
 ------------------------------ | ----------------------------------------------
--- | | System | `unit_id` | (none) | | | Partition | `uncleared_issues`,
-`desired_state` | arm away, arm stay, arm night, disarm | | | Sensor |
-`device_subtype` | (none) | | | Locks | `desired_state` | lock, unlock | | |
-Garage Door | (none) | open, close | | | Gate | `supports_remote_close` | open,
-close | | | Image Sensor | `images` | peek_in | | | Light | `brightness` |
-turn_on (with brightness), turn_off | No support for RGB/W, effects,
-temperature, etc. | | Thermostat | `temp_average`, `temp_at_tstat`,
-`step_value`, `supports_fan_mode`, `supports_fan_indefinite`,
+-- | | System | `unit_id` | (none) | | | Partition | `uncleared_issues` | arm
+away, arm stay, arm night, disarm | | | Sensor | `device_subtype` | (none) | |
+| Locks | | lock, unlock | | | Garage Door | (none) | open, close | | | Gate |
+`supports_remote_close` | open, close | | | Image Sensor | `images` | peek_in |
+| | Light | `brightness` | turn_on (with brightness), turn_off | No support for
+RGB/W, effects, temperature, etc. | | Thermostat | `temp_average`,
+`temp_at_tstat`, `step_value`, `supports_fan_mode`, `supports_fan_indefinite`,
 `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`,
 `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`,
 `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`,
 `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`,
 `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` |
 set_attribute | | | Water Sensor | | (none) | | ### Known Sensor deviceTypes
 This list identifies deviceTypes used in the alarm.com API and is incomplete.
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/__init__.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,56 +10,52 @@
 from datetime import datetime
 from enum import Enum
 from typing import TypedDict
 
 import aiohttp
 from bs4 import BeautifulSoup
 
-from pyalarmdotcomajax.devices.partition import Partition
-from pyalarmdotcomajax.devices.registry import AllDevices_t
-from pyalarmdotcomajax.websockets.client import WebSocketClient
-
-from . import const as c
-from .devices import (
+from pyalarmdotcomajax import const as c
+from pyalarmdotcomajax.devices import (
     BaseDevice,
     DeviceTypeSpecificData,
     TroubleCondition,
 )
-from .devices.registry import AttributeRegistry, DeviceRegistry, DeviceType
-from .errors import (
+from pyalarmdotcomajax.devices.partition import Partition
+from pyalarmdotcomajax.devices.registry import (
+    AllDevices_t,
+    AttributeRegistry,
+    DeviceRegistry,
+    DeviceType,
+)
+from pyalarmdotcomajax.errors import (
     AuthenticationFailed,
     DataFetchFailed,
-    NagScreen,
     TryAgain,
+    TwoFactor_ConfigurationRequired,
+    TwoFactor_OtpRequired,
     UnexpectedDataStructure,
     UnsupportedDevice,
 )
-from .extensions import (
+from pyalarmdotcomajax.extensions import (
     CameraSkybellControllerExtension,
     ConfigurationOption,
     ControllerExtensions_t,
     ExtendedProperties,
 )
+from pyalarmdotcomajax.websockets.client import WebSocketClient
 
 # TODO: Use error handler and exception handlers in _async_get_system_devices on other request functions.
 # TODO: Fix get raw server response function.
 
-__version__ = "0.5.0-beta.2"
+__version__ = "0.5.0-beta.3"
 
 log = logging.getLogger(__name__)
 
 
-class AuthResult(Enum):
-    """Standard for reporting results of login attempt."""
-
-    SUCCESS = "success"
-    OTP_REQUIRED = "otp_required"
-    ENABLE_TWO_FACTOR = "enable_two_factor"
-
-
 class ExtensionResults(TypedDict):
     """Results of multi-device extension calls."""
 
     settings: dict[str, ConfigurationOption]
     controller: ControllerExtensions_t
 
 
@@ -98,17 +94,15 @@
     LOGIN_2FA_POST_URL_TEMPLATE = (
         "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}/verifyTwoFactorCode"
     )
     LOGIN_2FA_DETAIL_URL_TEMPLATE = "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}"
     LOGIN_2FA_TRUST_URL_TEMPLATE = (
         "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}/trustTwoFactorDevice"
     )
-    LOGIN_2FA_REQUEST_OTP_SMS_URL_TEMPLATE = (
-        "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}/sendTwoFactorAuthenticationCode"
-    )
+    LOGIN_2FA_REQUEST_OTP_SMS_URL_TEMPLATE = "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}/sendTwoFactorAuthenticationCodeViaSms"
     LOGIN_2FA_REQUEST_OTP_EMAIL_URL_TEMPLATE = "{}web/api/engines/twoFactorAuthentication/twoFactorAuthentications/{}/sendTwoFactorAuthenticationCodeViaEmail"
 
     VIEWSTATE_FIELD = "__VIEWSTATE"
     VIEWSTATEGENERATOR_FIELD = "__VIEWSTATEGENERATOR"
     EVENTVALIDATION_FIELD = "__EVENTVALIDATION"
     PREVIOUSPAGE_FIELD = "__PREVIOUSPAGE"
 
@@ -135,16 +129,14 @@
         self._websession: aiohttp.ClientSession = websession
         self._two_factor_cookie: dict = {"twoFactorAuthenticationId": twofactorcookie} if twofactorcookie else {}
 
         #
         # INITIALIZE
         #
 
-        self._factor_type_id: int | None = None
-        self._two_factor_method: OtpType | None = None
         self._provider_name: str | None = None
         self._user_id: str | None = None
         self._user_email: str | None = None
         self._active_system_id: str | None = None
         self._ajax_headers: dict = self.AJAX_HEADERS_TEMPLATE
         self.notify_on_update_callback: Awaitable | None = notify_on_update_callback
 
@@ -205,53 +197,76 @@
     #
     ####################
     # PUBLIC FUNCTIONS #
     ####################
     #
     #
 
-    async def async_login(self, request_otp: bool = True) -> AuthResult:
+    async def async_login(
+        self,
+    ) -> None:
         """Login to Alarm.com."""
         log.debug("Attempting to log in to Alarm.com")
 
         # TODO: Prevent login from making a ton of saved devices in ADC.
 
         try:
             await self._async_login_and_get_key()
             await self._async_get_identity_info()
 
-            if not self._two_factor_cookie and await self._async_requires_2fa():
-                log.debug("Two factor authentication code or cookie required.")
-
-                if request_otp and self._two_factor_method in [
-                    OtpType.SMS,
-                    OtpType.EMAIL,
-                ]:
-                    await self.async_request_otp()
+            # Check whether two factor authentication is required.
+            if not self._two_factor_cookie:
+                async with self._websession.get(
+                    url=AttributeRegistry.get_endpoints(DeviceType.SYSTEM)["primary"].format(c.URL_BASE, ""),
+                    headers=self._ajax_headers,
+                ) as resp:
+                    json_rsp = await resp.json()
 
-                return AuthResult.OTP_REQUIRED
+                for error in (errors := json_rsp.get("errors", {})):
+                    if error.get("status") == "409" and error.get("detail") == "TwoFactorAuthenticationRequired":
+                        log.debug("Two factor authentication code or cookie required.")
+                        raise TwoFactor_OtpRequired
 
         except (DataFetchFailed, UnexpectedDataStructure) as err:
             raise ConnectionError from err
         except (AuthenticationFailed, PermissionError) as err:
             raise AuthenticationFailed from err
-        except NagScreen:
-            return AuthResult.ENABLE_TWO_FACTOR
+        except TwoFactor_ConfigurationRequired as err:
+            raise err
 
-        return AuthResult.SUCCESS
+        log.info("Logged in successfully.")
+        return None
 
-    async def async_request_otp(self) -> str | None:
+    async def async_get_enabled_2fa_methods(self) -> list[OtpType]:
+        """Get list of two factor authentication methods enabled on account."""
+
+        async with self._websession.get(
+            url=self.LOGIN_2FA_DETAIL_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
+            headers=self._ajax_headers,
+        ) as resp:
+            json_rsp = await resp.json()
+            enabled_otp_types_bitmask = json_rsp.get("data", {}).get("attributes", {}).get("enabledTwoFactorTypes")
+            enabled_2fa_methods = [
+                otp_type for otp_type in OtpType if bool(enabled_otp_types_bitmask & otp_type.value)
+            ]
+            log.info(f"Requires two-factor authentication. Enabled methods are {enabled_2fa_methods}")
+            return enabled_2fa_methods
+
+    async def async_request_otp(self, method: OtpType | None) -> None:
         """Request SMS/email OTP code from Alarm.com."""
 
+        if method not in (OtpType.EMAIL, OtpType.SMS):
+            return None
+
         try:
             log.debug("Requesting OTP code...")
 
             request_url = (
                 self.LOGIN_2FA_REQUEST_OTP_EMAIL_URL_TEMPLATE
-                if self._two_factor_method == OtpType.EMAIL
+                if method == OtpType.EMAIL
                 else self.LOGIN_2FA_REQUEST_OTP_SMS_URL_TEMPLATE
             )
 
             async with self._websession.post(
                 url=request_url.format(c.URL_BASE, self._user_id),
                 headers=self._ajax_headers,
             ) as resp:
@@ -260,31 +275,31 @@
 
         except (asyncio.TimeoutError, aiohttp.ClientError) as err:
             log.error("Can not load 2FA submission page from Alarm.com")
             raise DataFetchFailed from err
 
         return None
 
-    async def async_submit_otp(self, code: str, device_name: str | None = None) -> str | None:
+    async def async_submit_otp(self, code: str, method: OtpType, device_name: str | None = None) -> str | None:
         """Submit two factor authentication code.
 
         Register device and return 2FA code if device_name is not None.
         """
 
         # Submit code
         try:
             log.debug("Submitting OTP code...")
 
-            if not self._two_factor_method:
+            if not method:
                 raise AuthenticationFailed("Missing OTP type.")
 
             async with self._websession.post(
                 url=self.LOGIN_2FA_POST_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
                 headers=self._ajax_headers,
-                json={"code": code, "typeOf2FA": self._two_factor_method.value},
+                json={"code": code, "typeOf2FA": method.value},
             ) as resp:
                 json_rsp = await resp.json()
 
         except (asyncio.TimeoutError, aiohttp.ClientError) as err:
             log.error("Can not load 2FA submission page from Alarm.com")
             raise DataFetchFailed from err
 
@@ -816,56 +831,14 @@
 
         except (asyncio.TimeoutError, aiohttp.ClientError, aiohttp.ClientResponseError, KeyError) as err:
             log.error(f"Failed to get {device_type.value}.")
             raise DataFetchFailed from err
         except TryAgain:
             return await self._async_get_devices_by_device_type(device_type=device_type, retry_on_failure=False)
 
-    async def _async_unmask_otp(self, enabled_otp_types: int) -> OtpType:
-        """Extract single OTP type from enabledTwoFactorTypes bitmask."""
-
-        if bool(enabled_otp_types & OtpType.APP.value):
-            return OtpType.APP
-        elif bool(enabled_otp_types & OtpType.SMS.value):
-            return OtpType.SMS
-        elif bool(enabled_otp_types & OtpType.EMAIL.value):
-            return OtpType.EMAIL
-        else:
-            raise ValueError(f"Unknown OTP type: {enabled_otp_types}")
-
-    async def _async_requires_2fa(self) -> bool | None:
-        """Check whether two factor authentication is enabled on the account."""
-        async with self._websession.get(
-            url=AttributeRegistry.get_endpoints(DeviceType.SYSTEM)["primary"].format(c.URL_BASE, ""),
-            headers=self._ajax_headers,
-        ) as resp:
-            json_rsp = await resp.json()
-
-        if (errors := json_rsp.get("errors")) and len(errors) > 0:
-            for error in errors:
-                if error.get("status") == "409" and error.get("detail") == "TwoFactorAuthenticationRequired":
-                    log.debug("Two factor authentication is required. Getting details...")
-                    # Get 2FA type ID
-                    async with self._websession.get(
-                        url=self.LOGIN_2FA_DETAIL_URL_TEMPLATE.format(c.URL_BASE, self._user_id),
-                        headers=self._ajax_headers,
-                    ) as resp:
-                        json_rsp = await resp.json()
-
-                        if isinstance(factor_id := json_rsp.get("data", {}).get("id"), int):
-                            self._factor_type_id = factor_id
-                            self._two_factor_method = await self._async_unmask_otp(
-                                json_rsp.get("data", {}).get("attributes", {}).get("enabledTwoFactorTypes")
-                            )
-                            log.info("Requires 2FA. Using method %s", self._two_factor_method)
-                            return True
-
-        log.debug("Does not require 2FA.")
-        return False
-
     async def _async_get_identity_info(self) -> None:
         """Get user id, email address, provider name, etc."""
         try:
             async with self._websession.get(
                 url=c.IDENTITIES_URL_TEMPLATE.format(c.URL_BASE, ""),
                 headers=self._ajax_headers,
                 cookies=self._two_factor_cookie,
@@ -1049,15 +1022,15 @@
                     log.error("Login failed.")
                     log.error("\nResponse URL:\n%s\n", str(resp.url))
                     log.error("\nRequest Headers:\n%s\n", str(resp.request_info.headers))
                     raise AuthenticationFailed("Invalid username and password.")
 
                 # If Alarm.com is warning us that we'll have to set up two factor authentication soon, alert caller.
                 if re.search("concurrent-two-factor-authentication", str(resp.url)) is not None:
-                    raise NagScreen("Encountered 2FA nag screen.")
+                    raise TwoFactor_ConfigurationRequired("Encountered 2FA nag screen.")
 
                 # Update anti-forgery cookie
                 self._ajax_headers["ajaxrequestuniquekey"] = resp.cookies["afg"].value
 
         except (asyncio.TimeoutError, aiohttp.ClientError) as err:
             log.error("Can not login to Alarm.com")
             raise DataFetchFailed from err
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/cli.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """pyalarmdotcomajax CLI.
 
 Based on https://github.com/uvjustin/pyalarmdotcomajax/pull/16 by Kevin David (@kevin-david)
 """
 
-# ruff: noqa: T201
+# ruff: noqa: T201 C901
 
 from __future__ import annotations
 
 import argparse
 import asyncio
 import json
 import logging
 import platform
 import sys
+from collections.abc import Sequence
 from dataclasses import asdict
 from enum import Enum
 from typing import Any
 
 import aiohttp
 from termcolor import colored, cprint
 
 import pyalarmdotcomajax
 from pyalarmdotcomajax.devices.registry import AllDevices_t, AttributeRegistry
 
-from . import AlarmController, AuthResult
+from . import AlarmController, OtpType
 from .devices import BaseDevice, DeviceType
 from .devices.light import Light
 from .devices.sensor import Sensor
-from .devices.system import System
 from .errors import (
     InvalidConfigurationOption,
-    NagScreen,
+    TwoFactor_ConfigurationRequired,
+    TwoFactor_OtpRequired,
     UnexpectedDataStructure,
 )
 from .extensions import ConfigurationOption
 from .helpers import ExtendedEnumMixin, slug_to_title
 
 CLI_CARD_BREAK = ""  # "--------"
 
@@ -77,14 +78,22 @@
         default=0,
         required=False,
     )
     parser.add_argument("-u", "--username", dest="username", help="alarm.com username", required=True)
     parser.add_argument("-p", "--password", dest="password", help="alarm.com password", required=True)
 
     parser.add_argument(
+        "--otp-method",
+        help="preferred OTP method to use during login if multiple are enabled for user account. case sensitive.",
+        type=OtpType,
+        action=EnumAction,
+        required=False,
+    )
+
+    parser.add_argument(
         "-n",
         "--device-name",
         help=(
             "registers a device with this name on alarm.com and requests the two-factor authentication cookie for"
             " the device."
         ),
         required=False,
@@ -162,32 +171,32 @@
     set_subparser.add_argument(
         "-k",
         "--new-value",
         help="New value for setting.",
     )
 
     #
-    # WebSocket / Watch Subparser
+    # WebSocket / stream Subparser
     #
 
     get_subparser = subparsers.add_parser(
-        "watch",
+        "stream",
         description="monitor alarm.com for real time updates",
         help="monitor alarm.com for real time updates over WebSockets. hit Ctrl + C to exit.",
     )
 
     ##########
     # SET UP #
     ##########
 
     args = vars(parser.parse_args())
 
     if args.get("debug", 0) > 0:
         logging.basicConfig(level=logging.DEBUG)
-    elif args.get("action") == "watch":
+    elif args.get("action") == "stream":
         logging.basicConfig(level=logging.INFO)
     else:
         logging.basicConfig(level=logging.ERROR)
 
     ##########
     # LOG IN #
     ##########
@@ -206,49 +215,25 @@
         alarm = pyalarmdotcomajax.AlarmController(
             username=args.get("username", ""),
             password=args.get("password", ""),
             websession=session,
             twofactorcookie=args.get("cookie"),
         )
 
-        generated_2fa_cookie = None
-
         try:
-            login_result = await alarm.async_login()
-        except NagScreen:
+            await alarm.async_login()
+        except TwoFactor_ConfigurationRequired:
             cprint(
                 "Unable to log in. Please set up two-factor authentication for this account.",
                 "red",
             )
             sys.exit()
 
-        if login_result == AuthResult.OTP_REQUIRED:
-            code: str | None
-            if not (code := args.get("one_time_password")):
-                cprint(
-                    "Two factor authentication is enabled for this user.",
-                    attrs=["bold"],
-                )
-                code = input("Enter One-Time Password: ")
-
-            if code:
-                generated_2fa_cookie = await alarm.async_submit_otp(code=code, device_name=args.get("device_name"))
-            else:
-                cprint(
-                    "Not enough information provided to make a decision regarding two-factor authentication.",
-                    "red",
-                )
-                sys.exit()
-
-        if login_result == AuthResult.ENABLE_TWO_FACTOR:
-            cprint(
-                "Unable to log in. Please set up two-factor authentication for this account.",
-                "red",
-            )
-            sys.exit()
+        except TwoFactor_OtpRequired:
+            await async_handle_otp_workflow(alarm, args)
 
         #######################
         # REFRESH DEVICE DATA #
         #######################
 
         await alarm.async_update()
 
@@ -275,15 +260,16 @@
                             == AttributeRegistry.get_relationship_id_from_devicetype(device_type)
                         ]
                     )
                     else "\n(none found)\n"
                 )
                 for device_type in DeviceType
                 if (
-                    device_type in AttributeRegistry.supported_device_types
+                    device_type
+                    in AttributeRegistry.supported_device_types  # pylint: disable=unsupported-membership-test
                     or args.get("include_unsupported", False)
                 )
             }
 
             # TODO: Include Image Sensor Image Data
 
             # Get & Add Human Output
@@ -305,17 +291,14 @@
                     "grey",
                     "on_yellow",
                     attrs=["bold"],
                 )
                 print(device_type_body)
                 print("")
 
-            if generated_2fa_cookie:
-                cprint(f"\n2FA Cookie: {generated_2fa_cookie}\n", "green")
-
         ############################
         # SET DEVICE DATA WORKFLOW #
         ############################
 
         if args.get("action") == "set":
             try:
                 device_id: str = args["device_id"]
@@ -399,46 +382,50 @@
                 )
             else:
                 cprint(
                     f"Error changing {config_option.name} for {device.name}.",
                     "red",
                 )
 
-        ###########################
-        # WATCH REAL TIME UPDATES #
-        ###########################
+        ############################
+        # STREAM REAL TIME UPDATES #
+        ############################
 
-        if args.get("action") == "watch":
+        if args.get("action") == "stream":
             cprint(
-                "Watching for real-time updates...",
+                "Streaming real-time updates...",
                 "grey",
                 "on_yellow",
                 attrs=["bold"],
             )
-            await _async_watch_realtime(alarm)
+            cprint(
+                "(Press Ctrl+C or Cmd+C to exit.)",
+                attrs=["bold"],
+            )
+            await _async_stream_realtime(alarm)
 
 
 #############
 # FUNCTIONS #
 #############
 
 
-async def _async_watch_realtime(alarm: AlarmController) -> None:
-    """Watch for real-time updates via WebSockets."""
+async def _async_stream_realtime(alarm: AlarmController) -> None:
+    """Stream real-time updates via WebSockets."""
 
     ws_client = alarm.get_websocket_client()
     await ws_client.async_connect()
 
 
 def _human_output(alarm: AlarmController) -> dict:
     """Output user-friendly list of devices and statuses."""
 
     output = {}
 
-    for device_type in AttributeRegistry.supported_device_types:
+    for device_type in AttributeRegistry.supported_device_types:  # pylint: ignore=not-an-iterable
         devices: dict[str, AllDevices_t] = getattr(alarm.devices, AttributeRegistry.get_storage_name(device_type))
         device_type_output: str = ""
         if len(devices) == 0:
             device_type_output += "\n(none found)\n"
         else:
             for device in sorted(devices.values(), key=lambda device: str(device.name)):
                 device_type_output += _print_element_tearsheet(device)
@@ -467,30 +454,23 @@
     elif element.battery_low:
         battery = "Low"
     elif element.battery_critical is not None or element.battery_low is not None:
         battery = "Normal"
     else:
         battery = None
 
-    # DESIRED STATE
-    desired_str = (
-        f" (Desired: {element.desired_state.name})"
-        if isinstance(element, System) and element.desired_state
-        else ""
-    )
-
     # ATTRIBUTES
     output_str += "ATTRIBUTES: "
 
     if isinstance(element.device_subtype, Sensor.Subtype) or element.state or battery or element.read_only:
         if isinstance(element.device_subtype, Sensor.Subtype):
             output_str += f'[TYPE: {element.device_subtype.name.title().replace("_"," ")}] '
 
         if element.state:
-            output_str += f"[STATE: {element.state.name.title()}{desired_str}] "
+            output_str += f"[STATE: {element.state.name.title()}] "
 
         if battery:
             output_str += f"[BATTERY: {battery}] "
 
         if element.read_only:
             output_str += f"[READ ONLY: {element.read_only}] "
 
@@ -536,14 +516,111 @@
             output_str += f"""[TITLE: {condition["title"]}] [MESSAGE ID: {condition["message_id"]}] [MESSAGE: {condition["body"]}] """
 
         output_str += "\n"
 
     return output_str
 
 
+async def async_handle_otp_workflow(alarm: AlarmController, args: dict[str, Any]) -> None:
+    """Handle two-factor authentication workflow."""
+
+    #
+    # Determine which OTP method to use
+    #
+
+    code: str | None
+    selected_otp_method: OtpType
+    if code := args.get("one_time_password"):
+        # If an OTP is provided directly in the CLI, it's from an OTP app.
+        selected_otp_method = OtpType.APP
+    else:
+        cprint(
+            "Two factor authentication is enabled for this user.",
+            attrs=["bold"],
+        )
+
+        # Get list of enabled OTP methods.
+        if len(enabled_2fa_methods := await alarm.async_get_enabled_2fa_methods()) == 1:
+            # If only one OTP method is enabled, use it without prompting user.
+            selected_otp_method = enabled_2fa_methods[0]
+            cprint(f"Using {selected_otp_method.name} for One-Time Password.")
+        elif cli_otp_method := args.get("otp_method"):
+            # If multiple OTP methods are enabled, but the user provided one via CLI, use it.
+            selected_otp_method = OtpType(cli_otp_method)
+            cprint(f"Using {selected_otp_method.name} for One-Time Password.")
+        else:
+            # If multiple OTP methods are enabled, let the user pick.
+            cprint("\nAvailable one-time password methods:")
+            for otp_method in enabled_2fa_methods:
+                cprint(f"{otp_method.value}: {otp_method.name}")
+            if not (
+                selected_otp_method := OtpType(
+                    int(input("\nWhich OTP method would you like to use? Enter the method's number: "))
+                )
+            ):
+                cprint("Valid OTP method was not entered.", "red")
+                sys.exit()
+
+        #
+        # Request OTP
+        #
+
+        if selected_otp_method in (OtpType.EMAIL, OtpType.SMS):
+            # Ask Alarm.com to send OTP if selected method is EMAIL or SMS.
+            cprint(f"Requesting One-Time Password via {selected_otp_method.name}...")
+            await alarm.async_request_otp(selected_otp_method)
+
+    #
+    # Prompt user for OTP
+    #
+
+    if not (code := input("Enter One-Time Password: ")):
+        cprint("Requested OTP was not entered.", "red")
+        sys.exit()
+
+    await alarm.async_submit_otp(code=code, method=selected_otp_method)
+
+
+class EnumAction(argparse.Action):
+    """Argparse action for handling Enums.
+
+    via https://stackoverflow.com/a/60750535 by Tim
+    CC BY-SA 4.0 (https://creativecommons.org/licenses/by-sa/4.0/).
+    """
+
+    def __init__(self, **kwargs: Any) -> None:
+        """Initialize action."""
+        # Pop off the type value
+        enum_type = kwargs.pop("type", None)
+
+        # Ensure an Enum subclass is provided
+        if enum_type is None:
+            raise ValueError("type must be assigned an Enum when using EnumAction")
+        if not issubclass(enum_type, Enum):
+            raise TypeError("type must be an Enum when using EnumAction")
+
+        # Generate choices from the Enum
+        kwargs.setdefault("choices", tuple(e.name for e in enum_type if e != OtpType.DISABLED))
+
+        super().__init__(**kwargs)
+
+        self._enum = enum_type
+
+    def __call__(
+        self,
+        parser: argparse.ArgumentParser,
+        namespace: argparse.Namespace,
+        values: str | Sequence[Any] | None,
+        option_string: str | None = None,
+    ) -> None:
+        """Convert value back into an Enum."""
+        value = self._enum[values]
+        setattr(namespace, self.dest, value)
+
+
 def main() -> None:
     """Run primary CLI function via asyncio. Main entrypoint for command line tool."""
 
     # Below is necessary to prevent asyncio "Event loop is closed" error in Windows.
     if platform.system() == "Windows" and hasattr(asyncio, "WindowsSelectorEventLoopPolicy"):
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/__init__.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Alarm.com device base devices."""
 from __future__ import annotations
 
 import asyncio
 import logging
 from abc import ABC
-from collections.abc import Awaitable, Callable
+from collections.abc import Callable
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Protocol, TypedDict
+from typing import Any, TypedDict
 
 import aiohttp
 
 from pyalarmdotcomajax.errors import InvalidConfigurationOption, UnexpectedDataStructure
 from pyalarmdotcomajax.extensions import (
     CameraSkybellControllerExtension,
     ConfigurationOption,
@@ -63,65 +63,38 @@
 
     message_id: str
     title: str
     body: str
     device_id: str
 
 
-class DesiredStateProtocol(Protocol):
-    """Private variables for DesiredStateMixin."""
-
-    _attribs_raw: dict
-    desired_state: Enum | None
-    has_state: bool
-    state: Enum | None
-    DeviceState: type[Enum]
-
-
-class DesiredStateMixin:
-    """Mixin decorator for entities with desired_state attribute."""
-
-    @property
-    def desired_state(self: DesiredStateProtocol) -> Enum | None:
-        """Return state."""
-
-        try:
-            state: Enum = self.DeviceState(self._attribs_raw.get("desiredState"))
-        except (ValueError, TypeError):
-            return None
-
-        return state
-
-
 class DeviceTypeSpecificData(TypedDict, total=False):
     """Hold entity-type-specific metadata."""
 
     raw_recent_images: list[dict]
 
 
 class BaseDevice(ABC, CastingMixin):
     """Contains properties shared by all ADC devices."""
 
     _DEVICE_MODELS: dict  # deviceModelId: {"manufacturer": str, "model": str}
     _ATTRIB_STATE = "state"
 
-    ATTRIB_DESIRED_STATE = "desiredState"
-
     def __init__(
         self,
         id_: str,
         send_action_callback: Callable,
         config_change_callback: Callable | None,
         children: list[tuple[str, DeviceType]],
         raw_device_data: dict,
         device_type_specific_data: DeviceTypeSpecificData | None = None,
         trouble_conditions: list | None = None,
         partition_id: str | None = None,
         settings: dict | None = None,  # slug: ConfigurationOption
-        external_update_callback: Awaitable | None = None,  # Called when device is updated via WebSockets.
+        external_update_callback: Callable | None = None,  # Called when device is updated via WebSockets.
     ) -> None:
         """Initialize base element class."""
 
         self._id_: str = id_
         self._family_raw: str | None = raw_device_data.get("type")
         self._attribs_raw: dict = raw_device_data.get("attributes", {})
         self._device_type_specific_data: DeviceTypeSpecificData = (
@@ -134,15 +107,15 @@
         self.children = children
         self.trouble_conditions: list[TroubleCondition] = trouble_conditions if trouble_conditions else []
 
         self._system_id: str | None = (
             raw_device_data.get("relationships", {}).get("system", {}).get("data", {}).get("id")
         )
         self._partition_id: str | None = partition_id
-        self.external_update_callback: Awaitable | None = external_update_callback
+        self.external_update_callback: Callable | None = external_update_callback
 
         self.process_device_type_specific_data()
 
         log.debug("Initialized %s %s", self._family_raw, self.name)
 
     #
     # Properties
@@ -219,15 +192,15 @@
 
     @property
     def malfunction(self) -> bool | None:
         """Return whether device is malfunctioning."""
         return self._attribs_raw.get("isMalfunctioning", True) or self.state is None
 
     @property
-    def mac_address(self) -> bool | None:
+    def mac_address(self) -> str | None:
         """Return device MAC address."""
         return self._attribs_raw.get("macAddress")
 
     @property
     def raw_state_text(self) -> str | None:
         """Return state description as reported by ADC."""
         return self._attribs_raw.get("displayStateText")
@@ -267,32 +240,42 @@
         """Update device state when notified of externally-triggered change."""
 
         self._attribs_raw[self._ATTRIB_STATE] = raw_state
 
         log.info(f"{__name__} Got async update for {self.name} ({self.id_}) with new state: {self.state}.")
 
         if self.external_update_callback:
-            await self.external_update_callback
+            self.external_update_callback
 
     async def async_handle_external_attribute_change(self, new_attribute: dict) -> None:
         """Update device attribute when notified of externally-triggered change."""
 
         self._attribs_raw.update(new_attribute)
 
         if self.external_update_callback:
-            await self.external_update_callback
+            self.external_update_callback
 
     async def async_log_new_attribute(self, attribute_name: str, attribute_value: Any) -> None:
         """Log externally-triggered attribute change."""
 
         log.info(
             f"{__name__} Got async update for {self.name} ({self.id_}) with new {attribute_name}:"
             f" {attribute_value}."
         )
 
+    def register_external_update_callback(self, callback: Callable) -> None:
+        """Register callback to be called when device state changes."""
+
+        self.external_update_callback = callback
+
+    def unregister_external_update_callback(self) -> None:
+        """Unregister callback to be called when device state changes."""
+
+        self.external_update_callback = None
+
     # #
     # PLACEHOLDERS
     # #
 
     # All subclasses will have above functions. Only some will have the below and must be implemented as overloads.
     # Methods below are included here to silence mypy errors.
 
@@ -309,18 +292,14 @@
     class DeviceAttributes:
         """Hold non-primary device state attributes. To be overridden by children."""
 
     @property
     def attributes(self) -> DeviceAttributes | None:
         """Hold non-primary device state attributes. To be overridden by children."""
 
-    @property
-    def desired_state(self) -> Enum | None:
-        """Return state. To be overridden by children."""
-
     def process_device_type_specific_data(self) -> None:
         """Process element specific data. To be overridden by children."""
 
         return None
 
     async def async_change_setting(self, slug: str, new_value: Any) -> None:
         """Update specified configuration setting via extension."""
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/garage_door.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/garage_door.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from __future__ import annotations
 
 import logging
 from enum import Enum
 
 from pyalarmdotcomajax.devices import DeviceType
 
-from . import BaseDevice, DesiredStateMixin
+from . import BaseDevice
 
 log = logging.getLogger(__name__)
 
 
-class GarageDoor(DesiredStateMixin, BaseDevice):
+class GarageDoor(BaseDevice):
     """Represent Alarm.com garage door element."""
 
     class DeviceState(Enum):
         """Enum of garage door states."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/GarageDoorStatus.js
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/gate.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/gate.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 import logging
 from dataclasses import dataclass
 from enum import Enum
 
 from pyalarmdotcomajax.devices import DeviceType
 
-from . import BaseDevice, DesiredStateMixin
+from . import BaseDevice
 
 log = logging.getLogger(__name__)
 
 
-class Gate(DesiredStateMixin, BaseDevice):
+class Gate(BaseDevice):
     """Represent Alarm.com gate element."""
 
     @dataclass
     class GateAttributes(BaseDevice.DeviceAttributes):
         """Gate attributes."""
 
         supports_remote_close: bool | None  # Specifies whether the gate can be closed remotely.
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/image_sensor.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/image_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/light.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/light.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Alarm.com light."""
 from __future__ import annotations
 
 import logging
 from enum import Enum
 
-from pyalarmdotcomajax.devices import BaseDevice, DesiredStateMixin, DeviceType
+from pyalarmdotcomajax.devices import BaseDevice, DeviceType
 
 log = logging.getLogger(__name__)
 
 
 # WebSocket Handler: https://www.alarm.com/web/system/assets/customer-ember/websockets/handlers/lights.ts
-class Light(DesiredStateMixin, BaseDevice):
+class Light(BaseDevice):
     """Represent Alarm.com light element."""
 
     ATTRIB_LIGHT_LEVEL = "lightLevel"
 
     class DeviceState(Enum):
         """Enum of light states."""
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/lock.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/lock.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from __future__ import annotations
 
 import logging
 from enum import Enum
 
 from pyalarmdotcomajax.devices import DeviceType
 
-from . import BaseDevice, DesiredStateMixin
+from . import BaseDevice
 
 log = logging.getLogger(__name__)
 
 
-class Lock(DesiredStateMixin, BaseDevice):
+class Lock(BaseDevice):
     """Represent Alarm.com sensor element."""
 
     class DeviceState(Enum):
         """Enum of lock states."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/LockStatus.js
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/partition.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 import logging
 from dataclasses import dataclass
 from enum import Enum
 
 from pyalarmdotcomajax.devices import DeviceType
 
-from . import BaseDevice, DesiredStateMixin
+from . import BaseDevice
 
 log = logging.getLogger(__name__)
 
 
-class Partition(DesiredStateMixin, BaseDevice):
+class Partition(BaseDevice):
     """Represent Alarm.com partition element."""
 
     class ExtendedArmingOption(Enum):
         """Enum of extended arming options."""
 
         # https://www.alarm.com/web/system/assets/customer-ember/enums/ArmingOption.js
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/registry.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pyalarmdotcomajax.devices.light import Light
 from pyalarmdotcomajax.devices.lock import Lock
 from pyalarmdotcomajax.devices.partition import Partition
 from pyalarmdotcomajax.devices.sensor import Sensor
 from pyalarmdotcomajax.devices.system import System
 from pyalarmdotcomajax.devices.thermostat import Thermostat
 from pyalarmdotcomajax.devices.water_sensor import WaterSensor
-from pyalarmdotcomajax.errors import UnsupportedDevice
+from pyalarmdotcomajax.errors import UnkonwnDevice, UnsupportedDevice
 from pyalarmdotcomajax.helpers import classproperty
 
 log = logging.getLogger(__name__)
 
 AllDeviceTypes_t = (
     type[Camera]
     | type[GarageDoor]
@@ -107,18 +107,21 @@
     ############
 
     @property
     def all(self) -> dict[str, AllDevices_t]:
         """Return devices."""
         return self._devices
 
-    def get(self, device_id: str) -> AllDevices_t | None:
+    def get(self, device_id: str) -> AllDevices_t:
         """Get device by id."""
 
-        return self._devices.get(device_id)
+        try:
+            return self._devices[device_id]
+        except KeyError:
+            raise UnkonwnDevice(f"Device with id {device_id} not found.")
 
     def update(self, payload: dict[str, AllDevices_t], purge: bool = False) -> None:
         """Store device or list of devices."""
 
         if purge:
             self._devices = payload
         else:
@@ -380,25 +383,25 @@
         """Return device type from relationship id."""
         try:
             return AttributeRegistry._ATTRIBUTES[device_type]["rel_id"]
         except KeyError as err:
             raise UnsupportedDevice from err
 
     @classproperty
-    def supported_device_types(cls) -> list[DeviceType]:
+    def supported_device_types(cls) -> list[DeviceType]:  # pylint: disable=no-self-argument
         """Return list of supported devices."""
         return [device_type for device_type in cls._ATTRIBUTES if cls._ATTRIBUTES[device_type].get("class_")]
 
     @classproperty
-    def unsupported_device_types(cls) -> list[DeviceType]:
+    def unsupported_device_types(cls) -> list[DeviceType]:  # pylint: disable=no-self-argument
         """Return list of supported devices."""
         return [device_type for device_type in cls._ATTRIBUTES if not cls._ATTRIBUTES[device_type].get("class_")]
 
     @classproperty
-    def endpoints(cls) -> dict[DeviceType, DeviceTypeEndpoints]:
+    def endpoints(cls) -> dict[DeviceType, DeviceTypeEndpoints]:  # pylint: disable=no-self-argument
         """Return all endpoints for all device types."""
         return {device_type: cls.get_endpoints(device_type) for device_type in cls._ATTRIBUTES}
 
     @classproperty
-    def all_relationship_ids(cls) -> list[str]:
+    def all_relationship_ids(cls) -> list[str]:  # pylint: disable=no-self-argument
         """Return all relationship ids for all device types."""
         return [device_type["rel_id"] for device_type in cls._ATTRIBUTES.values()]
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/sensor.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/system.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/system.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/devices/thermostat.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/thermostat.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import logging
 from dataclasses import dataclass
 from enum import Enum
 
 from pyalarmdotcomajax.devices import DeviceType
 from pyalarmdotcomajax.errors import UnexpectedDataStructure
 
-from . import BaseDevice, DesiredStateMixin
+from . import BaseDevice
 
 log = logging.getLogger(__name__)
 
 
-class Thermostat(DesiredStateMixin, BaseDevice):
+class Thermostat(BaseDevice):
     """Represent Alarm.com thermostat element."""
 
     # Fan duration of 0 is indefinite. otherwise value == hours.
     # TODO: desiredRts (remote temp sensor), desiredLocalDisplayLockingMode. Need user with remote sensors.
     # In identity info, check localizeTempUnitsToCelsius.
 
     ATTRIB_SETPOINT_OFFSET = "setpointOffset"
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/errors.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     """pyalarmdotcomajax did not recognize the device ID."""
 
 
 class AuthenticationFailed(Exception):
     """Alarm.com authentication failure."""
 
 
-class TwoFactorAuthEnabled(Exception):
+class TwoFactor_OtpRequired(Exception):
     """User has two factor authentication enabled."""
 
 
-class NagScreen(Exception):
+class TwoFactor_ConfigurationRequired(Exception):
     """Client encountered Alarm.com nag screen to setup 2 factor authentication."""
 
 
 class DataFetchFailed(Exception):
     """General or connection error encountered when fetching data."""
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/extensions.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/helpers.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/helpers.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/client.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/client.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/const.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/const.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/__init__.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/garage_door.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/gate.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/light.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/light.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/lock.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/partition.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/sensor.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/thermostat.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/handler/water_sensor.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/water_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/websockets/messages.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/messages.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax/ws.py` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/ws.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax.egg-info/PKG-INFO` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.0b2
+Version: 0.5.0b3
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
@@ -67,17 +67,17 @@
 
 - As of v0.2, multiples of all devices are supported.
 - All devices include the attributes: `name`, `id_`, `state`, `battery_low`, `battery_critical`, `malfunctioning`, `parent_ids`, and a few others.
 
 | Device Type  | Notable Attributes                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Actions                               | Notes                                            |
 | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- | ------------------------------------------------ |
 | System       | `unit_id`                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | (none)                                |                                                  |
-| Partition    | `uncleared_issues`, `desired_state`                                                                                                                                                                                                                                                                                                                                                                                                                                       | arm away, arm stay, arm night, disarm |                                                  |
+| Partition    | `uncleared_issues`                                                                                                                                                                                                                                                                                                                                                                                                                                     | arm away, arm stay, arm night, disarm |                                                  |
 | Sensor       | `device_subtype`                                                                                                                                                                                                                                                                                                                                                                                                                                                          | (none)                                |                                                  |
-| Locks        | `desired_state`                                                                                                                                                                                                                                                                                                                                                                                                                                                           | lock, unlock                          |                                                  |
+| Locks        |                                                                                                                                                                                                                                                                                                                                                                                                                                                         | lock, unlock                          |                                                  |
 | Garage Door  | (none)                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | open, close                           |                                                  |
 | Gate         | `supports_remote_close`                                                                                                                                                                                                                                                                                                                                                                                                                                                   | open, close                           |                                                  |
 | Image Sensor | `images`                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | peek_in                               |                                                  |
 | Light        | `brightness`                                                                                                                                                                                                                                                                                                                                                                                                                                                              | turn_on (with brightness), turn_off   | No support for RGB/W, effects, temperature, etc. |
 | Thermostat   | `temp_average`, `temp_at_tstat`, `step_value`, `supports_fan_mode`, `supports_fan_indefinite`, `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`, `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`, `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`, `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`, `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` | set_attribute                         |                                                  |
 | Water Sensor |                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | (none)                                |                                                  |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b2 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b3 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
@@ -36,22 +36,21 @@
 ---- | ------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------------------------- | -------
 ------------------------------ | ----------------------------------------------
--- | | System | `unit_id` | (none) | | | Partition | `uncleared_issues`,
-`desired_state` | arm away, arm stay, arm night, disarm | | | Sensor |
-`device_subtype` | (none) | | | Locks | `desired_state` | lock, unlock | | |
-Garage Door | (none) | open, close | | | Gate | `supports_remote_close` | open,
-close | | | Image Sensor | `images` | peek_in | | | Light | `brightness` |
-turn_on (with brightness), turn_off | No support for RGB/W, effects,
-temperature, etc. | | Thermostat | `temp_average`, `temp_at_tstat`,
-`step_value`, `supports_fan_mode`, `supports_fan_indefinite`,
+-- | | System | `unit_id` | (none) | | | Partition | `uncleared_issues` | arm
+away, arm stay, arm night, disarm | | | Sensor | `device_subtype` | (none) | |
+| Locks | | lock, unlock | | | Garage Door | (none) | open, close | | | Gate |
+`supports_remote_close` | open, close | | | Image Sensor | `images` | peek_in |
+| | Light | `brightness` | turn_on (with brightness), turn_off | No support for
+RGB/W, effects, temperature, etc. | | Thermostat | `temp_average`,
+`temp_at_tstat`, `step_value`, `supports_fan_mode`, `supports_fan_indefinite`,
 `supports_fan_circulate_when_off`, `supported_fan_durations`, `fan_mode`,
 `supports_heat`, `supports_heat_aux`, `supports_cool`, `supports_auto`,
 `min_heat_setpoint`, `min_cool_setpoint`, `max_heat_setpoint`,
 `max_cool_setpoint`, `heat_setpoint`, `cool_setpoint`, `supports_humidity`,
 `humidity`, `supports_schedules`, `supports_schedules_smart`, `schedule_mode` |
 set_attribute | | | Water Sensor | | (none) | | ### Known Sensor deviceTypes
 This list identifies deviceTypes used in the alarm.com API and is incomplete.
```

### Comparing `pyalarmdotcomajax-0.5.0b2/pyalarmdotcomajax.egg-info/SOURCES.txt` & `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/setup.cfg` & `pyalarmdotcomajax-0.5.0b3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/tests/__init__.py` & `pyalarmdotcomajax-0.5.0b3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/tests/conftest.py` & `pyalarmdotcomajax-0.5.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/tests/test_controller.py` & `pyalarmdotcomajax-0.5.0b3/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/tests/test_device_extensions.py` & `pyalarmdotcomajax-0.5.0b3/tests/test_device_extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/tests/test_partition.py` & `pyalarmdotcomajax-0.5.0b3/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/tests/test_sensors.py` & `pyalarmdotcomajax-0.5.0b3/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b2/tests/test_thermostat.py` & `pyalarmdotcomajax-0.5.0b3/tests/test_thermostat.py`

 * *Files identical despite different names*

