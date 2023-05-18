# Comparing `tmp/IoTuring-2023.2.4.tar.gz` & `tmp/IoTuring-2023.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IoTuring-2023.2.4.tar", last modified: Wed Feb 15 16:56:34 2023, max compression
+gzip compressed data, was "IoTuring-2023.2.5.tar", last modified: Thu Feb 16 14:41:39 2023, max compression
```

## Comparing `IoTuring-2023.2.4.tar` & `IoTuring-2023.2.5.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.054761 IoTuring-2023.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.046761 IoTuring-2023.2.4/IoTuring/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.046761 IoTuring-2023.2.4/IoTuring/ClassManager/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/ClassManager/ClassManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/ClassManager/EntityClassManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/ClassManager/WarehouseClassManager.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/ClassManager/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.046761 IoTuring-2023.2.4/IoTuring/Configurator/
--rw-r--r--   0 runner    (1001) docker     (123)    19642 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Configurator/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Configurator/ConfiguratorIO.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Configurator/ConfiguratorLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Configurator/MenuPreset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.046761 IoTuring-2023.2.4/IoTuring/Entity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.042761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.046761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/ActiveWindow/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/ActiveWindow/ActiveWindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.046761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/AppInfo/
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/AppInfo/AppInfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.046761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Battery/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Battery/Battery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/BootTime/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/BootTime/BootTime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Cpu/Cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/DesktopEnvironment/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/DesktopEnvironment/DesktopEnvironment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Disk/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Disk/Disk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/DisplayMode/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/DisplayMode/DisplayMode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/FileSwitch/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/FileSwitch/FileSwitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Hostname/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Hostname/Hostname.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Lock/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Lock/Lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Monitor/
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Monitor/Monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Notify/
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Notify/Notify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Notify/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Os/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Os/Os.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Power/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Power/Power.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Ram/
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Ram/Ram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Temperature/
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Temperature/Temperature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Time/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Time/Time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Uptime/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Uptime/Uptime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Username/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Username/Username.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Volume/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Deployments/Volume/Volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/Entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/EntityData.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/EntityManager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.042761 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Brightness/
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Brightness/Brightness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/CpuTemperature/
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/CpuTemperature/CpuTemperatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Network/
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Network/Network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Screenshot/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Screenshot/Screenshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/State/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/State/State.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Terminal/
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Terminal/Terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Entity/ValueFormat/
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/ValueFormat/ValueFormatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/ValueFormat/ValueFormatterOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/ValueFormat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Entity/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Exceptions/Exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/Logger/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Logger/Colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Logger/LogObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Logger/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Logger/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.050761 IoTuring-2023.2.4/IoTuring/MyApp/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/MyApp/App.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.046761 IoTuring-2023.2.4/IoTuring/Protocols/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.054761 IoTuring-2023.2.4/IoTuring/Protocols/MQTTClient/
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Protocols/MQTTClient/MQTTClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Protocols/MQTTClient/TopicCallback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.054761 IoTuring-2023.2.4/IoTuring/Warehouse/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.046761 IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.054761 IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/ConsoleWarehouse/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/ConsoleWarehouse/ConsoleWarehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.054761 IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/
--rw-r--r--   0 runner    (1001) docker     (123)    15767 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/HomeAssistantWarehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/entities.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.054761 IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/MQTTWarehouse/
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/MQTTWarehouse/MQTTWarehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/Warehouse/Warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/IoTuring/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:56:34.046761 IoTuring-2023.2.4/IoTuring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50372 2023-02-15 16:56:34.000000 IoTuring-2023.2.4/IoTuring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-02-15 16:56:34.000000 IoTuring-2023.2.4/IoTuring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 16:56:34.000000 IoTuring-2023.2.4/IoTuring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-15 16:56:34.000000 IoTuring-2023.2.4/IoTuring.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-15 16:56:34.000000 IoTuring-2023.2.4/IoTuring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-15 16:56:34.000000 IoTuring-2023.2.4/IoTuring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    50372 2023-02-15 16:56:34.054761 IoTuring-2023.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-02-15 16:56:24.000000 IoTuring-2023.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 16:56:34.054761 IoTuring-2023.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.333029 IoTuring-2023.2.5/IoTuring/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.333029 IoTuring-2023.2.5/IoTuring/ClassManager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/ClassManager/ClassManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/ClassManager/EntityClassManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/ClassManager/WarehouseClassManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/ClassManager/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)    19642 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Configurator/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Configurator/ConfiguratorIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Configurator/ConfiguratorLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Configurator/MenuPreset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.329029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/ActiveWindow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/ActiveWindow/ActiveWindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/AppInfo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/AppInfo/AppInfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Battery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Battery/Battery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/BootTime/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/BootTime/BootTime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Cpu/Cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/DesktopEnvironment/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/DesktopEnvironment/DesktopEnvironment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Disk/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Disk/Disk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/DisplayMode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/DisplayMode/DisplayMode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/FileSwitch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/FileSwitch/FileSwitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Hostname/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Hostname/Hostname.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Lock/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Lock/Lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Monitor/Monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Notify/
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Notify/Notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Notify/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Os/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Os/Os.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Power/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Power/Power.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Ram/
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Ram/Ram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Temperature/Temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Time/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Time/Time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Uptime/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Uptime/Uptime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Username/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Username/Username.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Volume/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Deployments/Volume/Volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/Entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/EntityData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/EntityManager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.333029 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Brightness/Brightness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.337029 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/CpuTemperature/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/CpuTemperature/CpuTemperatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Network/
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Network/Network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Screenshot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Screenshot/Screenshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/State/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/State/State.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Terminal/Terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Entity/ValueFormat/
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/ValueFormat/ValueFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/ValueFormat/ValueFormatterOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/ValueFormat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Entity/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Exceptions/Exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Logger/Colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Logger/LogObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Logger/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Logger/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/MyApp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/MyApp/App.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.333029 IoTuring-2023.2.5/IoTuring/Protocols/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Protocols/MQTTClient/
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Protocols/MQTTClient/MQTTClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Protocols/MQTTClient/TopicCallback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Warehouse/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.333029 IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/ConsoleWarehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/ConsoleWarehouse/ConsoleWarehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)    15767 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/HomeAssistantWarehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/entities.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/MQTTWarehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/MQTTWarehouse/MQTTWarehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/Warehouse/Warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/IoTuring/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:41:39.333029 IoTuring-2023.2.5/IoTuring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50458 2023-02-16 14:41:39.000000 IoTuring-2023.2.5/IoTuring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-02-16 14:41:39.000000 IoTuring-2023.2.5/IoTuring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 14:41:39.000000 IoTuring-2023.2.5/IoTuring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-16 14:41:39.000000 IoTuring-2023.2.5/IoTuring.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-16 14:41:39.000000 IoTuring-2023.2.5/IoTuring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-16 14:41:39.000000 IoTuring-2023.2.5/IoTuring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    50458 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-16 14:41:29.000000 IoTuring-2023.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 14:41:39.341029 IoTuring-2023.2.5/setup.cfg
```

### Comparing `IoTuring-2023.2.4/COPYING` & `IoTuring-2023.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/ClassManager/ClassManager.py` & `IoTuring-2023.2.5/IoTuring/ClassManager/ClassManager.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Configurator/Configurator.py` & `IoTuring-2023.2.5/IoTuring/Configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Configurator/ConfiguratorIO.py` & `IoTuring-2023.2.5/IoTuring/Configurator/ConfiguratorIO.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Configurator/ConfiguratorLoader.py` & `IoTuring-2023.2.5/IoTuring/Configurator/ConfiguratorLoader.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Configurator/MenuPreset.py` & `IoTuring-2023.2.5/IoTuring/Configurator/MenuPreset.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/ActiveWindow/ActiveWindow.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/ActiveWindow/ActiveWindow.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/AppInfo/AppInfo.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/AppInfo/AppInfo.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Battery/Battery.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Battery/Battery.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Cpu/Cpu.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Cpu/Cpu.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/DesktopEnvironment/DesktopEnvironment.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/DesktopEnvironment/DesktopEnvironment.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Disk/Disk.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Disk/Disk.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/DisplayMode/DisplayMode.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/DisplayMode/DisplayMode.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/FileSwitch/FileSwitch.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/FileSwitch/FileSwitch.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Hostname/Hostname.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Hostname/Hostname.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Lock/Lock.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Lock/Lock.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Monitor/Monitor.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Monitor/Monitor.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Notify/Notify.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Notify/Notify.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Notify/icon.png` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Notify/icon.png`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Os/Os.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Os/Os.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Power/Power.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Power/Power.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Ram/Ram.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Ram/Ram.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Temperature/Temperature.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Temperature/Temperature.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,20 +189,20 @@
         for index, sensor in enumerate(self.getSensors()):
             if sensor.hasLabel():
                 label = sensor.getLabel()
             else:
                 label = FALLBACK_SENSOR_LABEL.format(index)
             if sensor.hasCurrent():
                 attributes[label +
-                           " - Current"] = str(sensor.getCurrent()) + "°C"
+                           " - Current"] = sensor.getCurrent()
             if sensor.hasHighest():
                 attributes[label +
-                           " - Highest"] = str(sensor.getHighest()) + "°C"
+                           " - Highest"] = sensor.getHighest()
             if sensor.hasCritical():
-                attributes[label + " - Critical"] = str(sensor.getCritical()) + "°C"
+                attributes[label + " - Critical"] = sensor.getCritical()
         return attributes
 
 
 class psutilTemperatureSensor():
     def __init__(self, sensorData) -> None:
         """ sensorData is an element from the list which is the value of the the dict returned by psutil.sensors_temperatures() """
         self.label = sensorData[0]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Uptime/Uptime.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Uptime/Uptime.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Username/Username.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Username/Username.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Deployments/Volume/Volume.py` & `IoTuring-2023.2.5/IoTuring/Entity/Deployments/Volume/Volume.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/Entity.py` & `IoTuring-2023.2.5/IoTuring/Entity/Entity.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/EntityData.py` & `IoTuring-2023.2.5/IoTuring/Entity/EntityData.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/EntityManager.py` & `IoTuring-2023.2.5/IoTuring/Entity/EntityManager.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Brightness/Brightness.py` & `IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Brightness/Brightness.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/ToImplement/CpuTemperature/CpuTemperatures.py` & `IoTuring-2023.2.5/IoTuring/Entity/ToImplement/CpuTemperature/CpuTemperatures.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Network/Network.py` & `IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Network/Network.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Screenshot/Screenshot.py` & `IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Screenshot/Screenshot.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/ToImplement/State/State.py` & `IoTuring-2023.2.5/IoTuring/Entity/ToImplement/State/State.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/ToImplement/Terminal/Terminal.py` & `IoTuring-2023.2.5/IoTuring/Entity/ToImplement/Terminal/Terminal.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/ValueFormat/ValueFormatter.py` & `IoTuring-2023.2.5/IoTuring/Entity/ValueFormat/ValueFormatter.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Entity/ValueFormat/ValueFormatterOptions.py` & `IoTuring-2023.2.5/IoTuring/Entity/ValueFormat/ValueFormatterOptions.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Logger/Logger.py` & `IoTuring-2023.2.5/IoTuring/Logger/Logger.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Logger/consts.py` & `IoTuring-2023.2.5/IoTuring/Logger/consts.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Protocols/MQTTClient/MQTTClient.py` & `IoTuring-2023.2.5/IoTuring/Protocols/MQTTClient/MQTTClient.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Protocols/MQTTClient/TopicCallback.py` & `IoTuring-2023.2.5/IoTuring/Protocols/MQTTClient/TopicCallback.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/ConsoleWarehouse/ConsoleWarehouse.py` & `IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/ConsoleWarehouse/ConsoleWarehouse.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/HomeAssistantWarehouse.py` & `IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/HomeAssistantWarehouse.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/entities.yaml` & `IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/entities.yaml`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Warehouse/Deployments/MQTTWarehouse/MQTTWarehouse.py` & `IoTuring-2023.2.5/IoTuring/Warehouse/Deployments/MQTTWarehouse/MQTTWarehouse.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/Warehouse/Warehouse.py` & `IoTuring-2023.2.5/IoTuring/Warehouse/Warehouse.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring/__init__.py` & `IoTuring-2023.2.5/IoTuring/__init__.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/IoTuring.egg-info/PKG-INFO` & `IoTuring-2023.2.5/IoTuring.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IoTuring
-Version: 2023.2.4
+Version: 2023.2.5
 Summary: Simple and powerful cross-platform script to control your pc and share statistics using communication protocols like MQTT and home control hubs like HomeAssistant.
 Author-email: richibrics <riccardo.briccola.dev@gmail.com>, infeeeee <gyetpet@mailbox.org>
 Maintainer-email: richibrics <riccardo.briccola.dev@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -678,15 +678,15 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: homepage, https://github.com/richibrics/IoTuring
 Project-URL: documentation, https://github.com/richibrics/IoTuring
 Project-URL: repository, https://github.com/richibrics/IoTuring
-Project-URL: changelog, https://github.com/richibrics/IoTuring/commits/main
+Project-URL: changelog, https://github.com/richibrics/IoTuring/releases
 Keywords: iot,mqtt,monitor
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -824,14 +824,15 @@
 | Os                 | shares the operating system of your machine                                 | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Power*             | commands for poweroff, reboot and sleep                                     | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Ram                | shares useful information about ram usage                                   | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Time               | shares the machine local time                                               | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Temperature        | shares temperature sensor data                                              | ![mac](docs/images/mac.png) ![linux](docs/images/linux.png)                             |
 | Uptime             | shares the time since the machine is on                                     | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Username           | shares the name of the user who is working on the machine                   | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
+| Volume           | control audio volume                | ![mac](docs/images/mac.png)  |
 
 \* To use the features from Power entity on Linux and macOS you need to give permissions to your user to shutdown and reboot without sudo password.
 You can easily do that by adding the following line at the end of the "/etc/sudoers" file (you can use the following command: sudo nano /etc/sudoers):
 
 ```
 YOURUSERNAMEHERE ALL=(ALL) NOPASSWD: /sbin/poweroff, /sbin/reboot, /sbin/shutdown
 ```
```

### Comparing `IoTuring-2023.2.4/IoTuring.egg-info/SOURCES.txt` & `IoTuring-2023.2.5/IoTuring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.2.4/PKG-INFO` & `IoTuring-2023.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IoTuring
-Version: 2023.2.4
+Version: 2023.2.5
 Summary: Simple and powerful cross-platform script to control your pc and share statistics using communication protocols like MQTT and home control hubs like HomeAssistant.
 Author-email: richibrics <riccardo.briccola.dev@gmail.com>, infeeeee <gyetpet@mailbox.org>
 Maintainer-email: richibrics <riccardo.briccola.dev@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -678,15 +678,15 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: homepage, https://github.com/richibrics/IoTuring
 Project-URL: documentation, https://github.com/richibrics/IoTuring
 Project-URL: repository, https://github.com/richibrics/IoTuring
-Project-URL: changelog, https://github.com/richibrics/IoTuring/commits/main
+Project-URL: changelog, https://github.com/richibrics/IoTuring/releases
 Keywords: iot,mqtt,monitor
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -824,14 +824,15 @@
 | Os                 | shares the operating system of your machine                                 | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Power*             | commands for poweroff, reboot and sleep                                     | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Ram                | shares useful information about ram usage                                   | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Time               | shares the machine local time                                               | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Temperature        | shares temperature sensor data                                              | ![mac](docs/images/mac.png) ![linux](docs/images/linux.png)                             |
 | Uptime             | shares the time since the machine is on                                     | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Username           | shares the name of the user who is working on the machine                   | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
+| Volume           | control audio volume                | ![mac](docs/images/mac.png)  |
 
 \* To use the features from Power entity on Linux and macOS you need to give permissions to your user to shutdown and reboot without sudo password.
 You can easily do that by adding the following line at the end of the "/etc/sudoers" file (you can use the following command: sudo nano /etc/sudoers):
 
 ```
 YOURUSERNAMEHERE ALL=(ALL) NOPASSWD: /sbin/poweroff, /sbin/reboot, /sbin/shutdown
 ```
```

### Comparing `IoTuring-2023.2.4/README.md` & `IoTuring-2023.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 | Os                 | shares the operating system of your machine                                 | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Power*             | commands for poweroff, reboot and sleep                                     | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Ram                | shares useful information about ram usage                                   | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Time               | shares the machine local time                                               | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Temperature        | shares temperature sensor data                                              | ![mac](docs/images/mac.png) ![linux](docs/images/linux.png)                             |
 | Uptime             | shares the time since the machine is on                                     | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
 | Username           | shares the name of the user who is working on the machine                   | ![win](docs/images/win.png) ![mac](docs/images/mac.png) ![linux](docs/images/linux.png) |
+| Volume           | control audio volume                | ![mac](docs/images/mac.png)  |
 
 \* To use the features from Power entity on Linux and macOS you need to give permissions to your user to shutdown and reboot without sudo password.
 You can easily do that by adding the following line at the end of the "/etc/sudoers" file (you can use the following command: sudo nano /etc/sudoers):
 
 ```
 YOURUSERNAMEHERE ALL=(ALL) NOPASSWD: /sbin/poweroff, /sbin/reboot, /sbin/shutdown
 ```
```

### Comparing `IoTuring-2023.2.4/pyproject.toml` & `IoTuring-2023.2.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "IoTuring"
-version = "2023.2.4"
+version = "2023.2.5"
 description = "Simple and powerful cross-platform script to control your pc and share statistics using communication protocols like MQTT and home control hubs like HomeAssistant."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "COPYING"}
 keywords = ["iot","mqtt","monitor"]
 authors = [
   {name = "richibrics", email = "riccardo.briccola.dev@gmail.com"},
@@ -30,15 +30,15 @@
   "tinyWinToast; sys_platform == 'win32'"
 ]
 
 [project.urls]
 homepage = "https://github.com/richibrics/IoTuring"
 documentation = "https://github.com/richibrics/IoTuring"
 repository = "https://github.com/richibrics/IoTuring"
-changelog = "https://github.com/richibrics/IoTuring/commits/main"
+changelog = "https://github.com/richibrics/IoTuring/releases"
 
 [project.scripts]
 IoTuring = "IoTuring:loop"
 
 [build-system]
 requires = ["setuptools", "wheel"]
```

