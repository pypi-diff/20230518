# Comparing `tmp/netbox-cisco-maintenance-0.0.2.tar.gz` & `tmp/netbox-cisco-maintenance-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-maintenance-0.0.2.tar", last modified: Thu May 18 14:08:29 2023, max compression
+gzip compressed data, was "netbox-cisco-maintenance-0.0.3.tar", last modified: Thu May 18 14:48:40 2023, max compression
```

## Comparing `netbox-cisco-maintenance-0.0.2.tar` & `netbox-cisco-maintenance-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4674 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.344314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/
--rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      657 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.344314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/commands/sync_eox_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)     1475 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0001_initial.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1410 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py
--rw-r--r--   0 vsts      (1001) docker     (123)      413 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0004_ciscosupport_is_covered.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1638 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py
--rw-r--r--   0 vsts      (1001) docker     (123)      605 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3180 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1820 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.344314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/netbox_cisco_support/
--rw-r--r--   0 vsts      (1001) docker     (123)     1286 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     2446 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device_type.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:08:29.344314 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-18 14:08:29.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1323 2023-05-18 14:08:29.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 14:08:29.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 14:08:29.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-18 14:08:29.000000 netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-18 14:08:29.348314 netbox-cisco-maintenance-0.0.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1538 2023-05-18 14:08:11.000000 netbox-cisco-maintenance-0.0.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:40.702767 netbox-cisco-maintenance-0.0.3/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-18 14:48:40.702767 netbox-cisco-maintenance-0.0.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4674 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:40.702767 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/
+-rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      657 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:40.702767 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:40.702767 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19710 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/management/commands/sync_eox_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:40.702767 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1475 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1410 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1153 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      413 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/0004_ciscosupport_is_covered.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1638 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      605 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3180 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1820 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:40.698767 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:40.702767 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/templates/netbox_cisco_support/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1286 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     2446 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device_type.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:40.702767 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:48:40.702767 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5296 2023-05-18 14:48:40.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1323 2023-05-18 14:48:40.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 14:48:40.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 14:48:40.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-05-18 14:48:40.000000 netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-18 14:48:40.702767 netbox-cisco-maintenance-0.0.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1538 2023-05-18 14:48:20.000000 netbox-cisco-maintenance-0.0.3/setup.py
```

### Comparing `netbox-cisco-maintenance-0.0.2/LICENSE` & `netbox-cisco-maintenance-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/PKG-INFO` & `netbox-cisco-maintenance-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.2
+Version: 0.0.3
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.2/README.md` & `netbox-cisco-maintenance-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/__init__.py` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/admin.py` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/management/commands/sync_eox_data.py` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/management/commands/sync_eox_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,27 +343,32 @@
 
         return serial_numbers
 
     def logon(self):
         PLUGIN_SETTINGS = settings.PLUGINS_CONFIG.get("netbox_cisco_maintenance", dict())
         CISCO_CLIENT_ID = PLUGIN_SETTINGS.get("cisco_client_id", "")
         CISCO_CLIENT_SECRET = PLUGIN_SETTINGS.get("cisco_client_secret", "")
+        # Set the requests timeout for connect and read separatly
+        REQUESTS_TIMEOUT = (3.05, 27)
 
-        token_url = "https://cloudsso.cisco.com/as/token.oauth2"
-        data = {
+        token_url = "https://id.cisco.com/oauth2/default/v1/token"
+        params = {
             "grant_type": "client_credentials",
             "client_id": CISCO_CLIENT_ID,
             "client_secret": CISCO_CLIENT_SECRET,
         }
+        headers = {"Content-Type": "application/x-www-form-urlencoded"}
 
-        access_token_response = requests.post(token_url, data=data)
+        access_token_response = requests.post(
+            url=token_url, params=params, headers=headers, timeout=REQUESTS_TIMEOUT
+        )
 
-        tokens = json.loads(access_token_response.text)
+        token = access_token_response.json()["access_token"]
 
-        api_call_headers = {"Authorization": "Bearer " + tokens["access_token"], "Accept": "application/json"}
+        api_call_headers = {"Authorization": "Bearer " + token, "Accept": "application/json"}
 
         return api_call_headers
 
     # Main entry point for the sync_eox_data command of manage.py
     def handle(self, *args, **kwargs):
         PLUGIN_SETTINGS = settings.PLUGINS_CONFIG.get("netbox_cisco_maintenance", dict())
         MANUFACTURER = PLUGIN_SETTINGS.get("manufacturer", "Cisco")
@@ -374,16 +379,15 @@
         # Step 1: Get all PIDs for all Device Types of that particular manufacturer
         product_ids = self.get_product_ids(MANUFACTURER)
         self.stdout.write(self.style.SUCCESS("Gathering data for these PIDs: " + ", ".join(product_ids)))
 
         i = 1
         for pid in product_ids:
             url = (
-                "https://api.cisco.com/supporttools/eox/rest/5/EOXByProductID/1/%s?responseencoding=json"
-                % pid
+                f"https://apix.cisco.com/supporttools/eox/rest/5/EOXByProductID/1/{pid}?responseencoding=json"
             )
             api_call_response = requests.get(url, headers=api_call_headers)
             self.stdout.write(self.style.SUCCESS("Call " + url))
 
             # sanatize file name
             filename = django.utils.text.get_valid_filename("%s.json" % pid)
 
@@ -415,15 +419,15 @@
         while serial_numbers:
             # Pop the first items_to_fetch items of serial_numbers into current_slice and then delete them from serial
             # numbers. We want to pass x items to the API each time we call it
             items_to_fetch = 10
             current_slice = serial_numbers[:items_to_fetch]
             serial_numbers[:items_to_fetch] = []
 
-            url = "https://api.cisco.com/sn2info/v2/coverage/summary/serial_numbers/%s" % ",".join(
+            url = "https://apix.cisco.com/sn2info/v2/coverage/summary/serial_numbers/%s" % ",".join(
                 current_slice
             )
             api_call_response = requests.get(url, headers=api_call_headers)
             self.stdout.write(self.style.SUCCESS("Call " + url))
 
             # Validate response from Cisco
             if api_call_response.status_code == 200:
```

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0001_initial.py` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/0002_ciscodevicetypesupport.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/0003_auto_20210722_1917.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/0005_auto_20210914_1344.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/migrations/0006_auto_20210921_0941.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/models.py` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/models.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/template_content.py` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device.html` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device_type.html` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/templates/netbox_cisco_support/cisco_support_device_type.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance/templatetags/filters.py` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/PKG-INFO` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-maintenance
-Version: 0.0.2
+Version: 0.0.3
 Summary: Implementing Cisco maintenance information with the Cisco Support APIs into NetBox
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-maintenance-0.0.2/netbox_cisco_maintenance.egg-info/SOURCES.txt` & `netbox-cisco-maintenance-0.0.3/netbox_cisco_maintenance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-cisco-maintenance-0.0.2/setup.py` & `netbox-cisco-maintenance-0.0.3/setup.py`

 * *Files identical despite different names*

