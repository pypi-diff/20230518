# Comparing `tmp/netbox-cisco-maintenance-0.0.1.tar.gz` & `tmp/netbox-cisco-maintenance-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-maintenance-0.0.1.tar", last modified: Thu May 18 13:23:37 2023, max compression
+gzip compressed data, was "netbox-cisco-maintenance-0.0.2.tar", last modified: Thu May 18 14:08:29 2023, max compression
```

## Comparing `netbox-cisco-maintenance-0.0.1.tar` & `netbox-cisco-maintenance-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:37.682211 netbox-cisco-maintenance-0.0.1/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     5473 2023-05-18 13:23:37.682211 netbox-cisco-maintenance-0.0.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4851 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:37.678211 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/
--rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      657 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:37.682211 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:37.682211 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/management/commands/sync_eox_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:37.682211 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)     1475 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/0001_initial.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1410 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py
--rw-r--r--   0 vsts      (1001) docker     (123)      413 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/0004_ciscosupport_is_covered.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1638 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py
--rw-r--r--   0 vsts      (1001) docker     (123)      605 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3180 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1820 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:37.678211 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:37.682211 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/templates/netbox_cisco_support/
--rw-r--r--   0 vsts      (1001) docker     (123)     1286 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     2446 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device_type.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:37.682211 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/templatetags/filters.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 13:23:37.682211 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5473 2023-05-18 13:23:37.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1287 2023-05-18 13:23:37.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 13:23:37.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 13:23:37.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-18 13:23:37.000000 netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-18 13:23:37.682211 netbox-cisco-maintenance-0.0.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1028 2023-05-18 13:23:17.000000 netbox-cisco-maintenance-0.0.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4674 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.344314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/
+-rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      657 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.344314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/commands/sync_eox_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1475 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1410 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      413 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0004_ciscosupport_is_covered.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1638 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      605 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3180 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1820 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.344314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/netbox_cisco_support/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1286 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     2446 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device_type.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.344314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-18 14:08:29.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1323 2023-05-18 14:08:29.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 14:08:29.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 14:08:29.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-18 14:08:29.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1538 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/setup.py
```

### Comparing `netbox-cisco-maintenance-0.0.1/LICENSE` & `netbox-cisco-maintenance-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/PKG-INFO` & `netbox-cisco-maintenance-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,23 @@
-Metadata-Version: 2.1
-Name: netbox-cisco-maintenance
-Version: 0.0.1
-Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
-Author: Willi Kubny
-Author-email: willi.kubny@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: System :: Networking
-Classifier: Topic :: System :: Systems Administration
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# NetBox Cisco Support API Plugin
-[NetBox](https://github.com/netbox-community/netbox) plugin using Cisco Support APIs to gather EoX and Contract coverage information for Cisco devices.
+# NetBox Cisco Maintenance
+[NetBox](https://github.com/netbox-community/netbox) plugin to show Cisco maintenance and software release data.
 
 ## Compatibility
-This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 3.0.3 and later.
+This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 3.5.0 and later.
 
 ## Installation
 The plugin is available as a Python package in pypi and can be installed with pip
 
-```
-$ source /opt/netbox/venv/bin/activate
-(venv) $ pip install netbox_cisco_maintenance
+```bash
+pip install netbox_cisco_maintenance
 ```
 
 Enable the plugin in `/opt/netbox/netbox/netbox/configuration.py`:
 
-```
+```python
 # Enable installed plugins. Add the name of each plugin to the list.
 PLUGINS = ['netbox_cisco_maintenance']
 
 # Plugins configuration settings. These settings are used by various plugins that the user may have installed.
 # Each key in the dictionary is the name of an installed plugin and its value is a dictionary of settings.
 PLUGINS_CONFIG = {
     'netbox_cisco_maintenance': {
@@ -43,53 +25,52 @@
         'cisco_client_secret': 'bazz' # Client Secret of your plugin installation. Generate it inside Cisco API Console
     }
 }
 ```
 
 Restart NetBox and add `netbox-cisco-maintenance` to your `local_requirements.txt`
 
-```
-(venv) $ cd /opt/netbox/netbox/
-(venv) $ python3 manage.py migrate
-# sudo systemctl restart netbox
+```bash
+python3 manage.py migrate
 ```
 
 Sync Cisco EoX data for the first time
+```bash
+python3 manage.py sync_eox_data
 ```
-(venv) $ cd /opt/netbox/netbox/
-(venv) $ python3 manage.py sync_eox_data
-````
 
 To periodically refresh EoX data create a cronjob which calls `sync_eox_data` periodically
-```
+```bash
 $ cat /etc/cron.d/netbox_sync_eox_data
 
 # Update Cisco EoX Data every Saturday at 14:03
 MAILTO="mail@example.com"
 3 14 * * 6 root /opt/netbox/venv/bin/python3 /opt/netbox/netbox/manage.py sync_eox_data
 ```
 
-or log into /tmp file
-```
+Or log into /tmp file
+```bash
 $ cat /etc/cron.d/netbox_sync_eox_data
 
 # Update Cisco EoX Data every Saturday at 14:03
 3 14 * * 6 root /opt/netbox/venv/bin/python3 /opt/netbox/netbox/manage.py sync_eox_data > /tmp/netbox_sync_eox_data
 ```
 
 ## Configuration
 The following options are available:
-* `cisco_client_id`: String - Client ID of your plugin installation. Generate it inside [Cisco API Console](https://apiconsole.cisco.com/)
-* `cisco_client_secret`: String - Client Secret of your plugin installation. Generate it inside [Cisco API Console](https://apiconsole.cisco.com/)
+* `cisco_client_id`: String - Client ID of your plugin installation.
+Generate it inside [Cisco API Console](https://apiconsole.cisco.com/)
+* `cisco_client_secret`: String - Client Secret of your plugin installation.
+Generate it inside [Cisco API Console](https://apiconsole.cisco.com/)
 
 ## Requirements
 In order to get the correct data using the API, several requirements must be fulfilled:
 1. A [Cisco API ID and secret](https://apiconsole.cisco.com/) (with access to the APIs "EOX V5 API" and "Serial Number to Information API Version 2") must have been created and configured inside `configuration.py`
 2. A manufacturer called `Cisco` must have been configured inside NetBox. If your manufacturer is named differently, change if inside `configuration.py`:
-```
+```python
 PLUGINS_CONFIG = {
     'netbox_cisco_maintenance': {
         ...,
         'manufacturer': 'Cisco Systems' # Optional setting for definiing the manufacturer
     }
 }
 ```
```

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/__init__.py` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/admin.py` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/management/commands/sync_eox_data.py` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/commands/sync_eox_data.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/0001_initial.py` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/models.py` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/models.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/template_content.py` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device.html` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device_type.html` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device_type.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance/templatetags/filters.py` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance.egg-info/PKG-INFO` & `netbox-cisco-maintenance-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.1
+Version: 0.0.2
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# NetBox Cisco Support API Plugin
-[NetBox](https://github.com/netbox-community/netbox) plugin using Cisco Support APIs to gather EoX and Contract coverage information for Cisco devices.
+# NetBox Cisco Maintenance
+[NetBox](https://github.com/netbox-community/netbox) plugin to show Cisco maintenance and software release data.
 
 ## Compatibility
-This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 3.0.3 and later.
+This plugin in compatible with [NetBox](https://netbox.readthedocs.org/) 3.5.0 and later.
 
 ## Installation
 The plugin is available as a Python package in pypi and can be installed with pip
 
-```
-$ source /opt/netbox/venv/bin/activate
-(venv) $ pip install netbox_cisco_maintenance
+```bash
+pip install netbox_cisco_maintenance
 ```
 
 Enable the plugin in `/opt/netbox/netbox/netbox/configuration.py`:
 
-```
+```python
 # Enable installed plugins. Add the name of each plugin to the list.
 PLUGINS = ['netbox_cisco_maintenance']
 
 # Plugins configuration settings. These settings are used by various plugins that the user may have installed.
 # Each key in the dictionary is the name of an installed plugin and its value is a dictionary of settings.
 PLUGINS_CONFIG = {
     'netbox_cisco_maintenance': {
@@ -43,53 +42,52 @@
         'cisco_client_secret': 'bazz' # Client Secret of your plugin installation. Generate it inside Cisco API Console
     }
 }
 ```
 
 Restart NetBox and add `netbox-cisco-maintenance` to your `local_requirements.txt`
 
-```
-(venv) $ cd /opt/netbox/netbox/
-(venv) $ python3 manage.py migrate
-# sudo systemctl restart netbox
+```bash
+python3 manage.py migrate
 ```
 
 Sync Cisco EoX data for the first time
+```bash
+python3 manage.py sync_eox_data
 ```
-(venv) $ cd /opt/netbox/netbox/
-(venv) $ python3 manage.py sync_eox_data
-````
 
 To periodically refresh EoX data create a cronjob which calls `sync_eox_data` periodically
-```
+```bash
 $ cat /etc/cron.d/netbox_sync_eox_data
 
 # Update Cisco EoX Data every Saturday at 14:03
 MAILTO="mail@example.com"
 3 14 * * 6 root /opt/netbox/venv/bin/python3 /opt/netbox/netbox/manage.py sync_eox_data
 ```
 
-or log into /tmp file
-```
+Or log into /tmp file
+```bash
 $ cat /etc/cron.d/netbox_sync_eox_data
 
 # Update Cisco EoX Data every Saturday at 14:03
 3 14 * * 6 root /opt/netbox/venv/bin/python3 /opt/netbox/netbox/manage.py sync_eox_data > /tmp/netbox_sync_eox_data
 ```
 
 ## Configuration
 The following options are available:
-* `cisco_client_id`: String - Client ID of your plugin installation. Generate it inside [Cisco API Console](https://apiconsole.cisco.com/)
-* `cisco_client_secret`: String - Client Secret of your plugin installation. Generate it inside [Cisco API Console](https://apiconsole.cisco.com/)
+* `cisco_client_id`: String - Client ID of your plugin installation.
+Generate it inside [Cisco API Console](https://apiconsole.cisco.com/)
+* `cisco_client_secret`: String - Client Secret of your plugin installation.
+Generate it inside [Cisco API Console](https://apiconsole.cisco.com/)
 
 ## Requirements
 In order to get the correct data using the API, several requirements must be fulfilled:
 1. A [Cisco API ID and secret](https://apiconsole.cisco.com/) (with access to the APIs "EOX V5 API" and "Serial Number to Information API Version 2") must have been created and configured inside `configuration.py`
 2. A manufacturer called `Cisco` must have been configured inside NetBox. If your manufacturer is named differently, change if inside `configuration.py`:
-```
+```python
 PLUGINS_CONFIG = {
     'netbox_cisco_maintenance': {
         ...,
         'manufacturer': 'Cisco Systems' # Optional setting for definiing the manufacturer
     }
 }
 ```
```

### Comparing `netbox-cisco-maintenance-0.0.1/netbox_cisco_maintenance.egg-info/SOURCES.txt` & `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.py
 netbox_cisco_maintenance/__init__.py
 netbox_cisco_maintenance/admin.py
 netbox_cisco_maintenance/models.py
 netbox_cisco_maintenance/template_content.py
+netbox_cisco_maintenance/version.py
 netbox_cisco_maintenance.egg-info/PKG-INFO
 netbox_cisco_maintenance.egg-info/SOURCES.txt
 netbox_cisco_maintenance.egg-info/dependency_links.txt
 netbox_cisco_maintenance.egg-info/not-zip-safe
 netbox_cisco_maintenance.egg-info/top_level.txt
 netbox_cisco_maintenance/management/__init__.py
 netbox_cisco_maintenance/management/commands/__init__.py
```

### Comparing `netbox-cisco-maintenance-0.0.1/setup.py` & `netbox-cisco-maintenance-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 #!/usr/bin/env python3
 """Build the netbox-cisco-maintenance Python Package with setuptools"""
 
+import codecs
+import os.path
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+def read(rel_path):
+    here = os.path.abspath(os.path.dirname(__file__))
+    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
+        return fp.read()
+
+def get_version(rel_path):
+    for line in read(rel_path).splitlines():
+        if line.startswith("__version__"):
+            delim = '"' if '"' in line else "'"
+            return line.split(delim)[1]
+    else:
+        raise RuntimeError("Unable to find version string.")
+
 setup(
     name="netbox-cisco-maintenance",
-    version="0.0.1",
+    version=get_version("netbox_cisco_maintenance/version.py"),
     author="Willi Kubny",
     author_email="willi.kubny@gmail.com",
     description="Implementing Cisco maintenance information with the Cisco Support APIs into NetBox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

