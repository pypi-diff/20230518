# Comparing `tmp/bpkio_python_sdk-1.0.1.tar.gz` & `tmp/bpkio_python_sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_python_sdk-1.0.1.tar", max compression
+gzip compressed data, was "bpkio_python_sdk-1.1.0.tar", max compression
```

## Comparing `bpkio_python_sdk-1.0.1.tar` & `bpkio_python_sdk-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.0.1/README.md
--rw-r--r--   0        0        0      157 2023-04-30 20:17:04.062783 bpkio_python_sdk-1.0.1/bpkio_api/__init__.py
--rw-r--r--   0        0        0     4729 2023-04-30 21:32:30.392195 bpkio_python_sdk-1.0.1/bpkio_api/api.py
--rw-r--r--   0        0        0     1044 2023-04-20 16:56:18.119327 bpkio_python_sdk-1.0.1/bpkio_api/caching.py
--rw-r--r--   0        0        0     3636 2023-04-30 21:16:38.524009 bpkio_python_sdk-1.0.1/bpkio_api/credential_provider.py
--rw-r--r--   0        0        0       34 2023-04-30 20:15:10.400387 bpkio_python_sdk-1.0.1/bpkio_api/defaults.py
--rw-r--r--   0        0        0      393 2023-04-07 16:54:49.526444 bpkio_python_sdk-1.0.1/bpkio_api/endpoints/__init__.py
--rw-r--r--   0        0        0     4379 2023-05-12 07:24:24.240126 bpkio_python_sdk-1.0.1/bpkio_api/endpoints/categories.py
--rw-r--r--   0        0        0      658 2023-04-14 21:22:20.218915 bpkio_python_sdk-1.0.1/bpkio_api/endpoints/consumption.py
--rw-r--r--   0        0        0    21134 2023-05-12 07:24:24.240807 bpkio_python_sdk-1.0.1/bpkio_api/endpoints/services.py
--rw-r--r--   0        0        0    21061 2023-05-12 07:24:24.241549 bpkio_python_sdk-1.0.1/bpkio_api/endpoints/sources.py
--rw-r--r--   0        0        0     2667 2023-05-12 07:24:24.242152 bpkio_python_sdk-1.0.1/bpkio_api/endpoints/tenants.py
--rw-r--r--   0        0        0     5713 2023-05-12 07:24:24.242673 bpkio_python_sdk-1.0.1/bpkio_api/endpoints/transcoding_profiles.py
--rw-r--r--   0        0        0     2619 2023-05-12 07:24:24.243027 bpkio_python_sdk-1.0.1/bpkio_api/endpoints/users.py
--rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.0.1/bpkio_api/exceptions.py
--rw-r--r--   0        0        0     2449 2023-04-29 21:37:29.834823 bpkio_python_sdk-1.0.1/bpkio_api/helpers/codecstrings.py
--rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/__init__.py
--rw-r--r--   0        0        0     4562 2023-05-05 10:37:16.925090 bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/dash.py
--rw-r--r--   0        0        0     3333 2023-05-04 10:23:23.525504 bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/factory.py
--rw-r--r--   0        0        0     1948 2023-05-02 20:36:39.412636 bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/generic.py
--rw-r--r--   0        0        0     4436 2023-05-12 07:24:24.255823 bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/hls.py
--rw-r--r--   0        0        0      436 2023-04-24 19:35:00.162089 bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/jpeg.py
--rw-r--r--   0        0        0      462 2023-04-24 19:37:38.335538 bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/mp4.py
--rw-r--r--   0        0        0      424 2023-04-24 19:36:40.587083 bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/png.py
--rw-r--r--   0        0        0     1956 2023-04-28 20:35:58.216707 bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/vast.py
--rw-r--r--   0        0        0     2305 2023-05-04 18:59:29.593036 bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/vmap.py
--rw-r--r--   0        0        0      560 2023-04-25 14:32:14.371116 bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/xml.py
--rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.0.1/bpkio_api/helpers/list.py
--rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.0.1/bpkio_api/helpers/objects.py
--rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.0.1/bpkio_api/helpers/profile_generator/__init__.py
--rw-r--r--   0        0        0      461 2023-04-30 19:12:24.858790 bpkio_python_sdk-1.0.1/bpkio_api/helpers/profile_generator/analyser.py
--rw-r--r--   0        0        0     1713 2023-04-29 21:41:55.874476 bpkio_python_sdk-1.0.1/bpkio_api/helpers/profile_generator/dash.py
--rw-r--r--   0        0        0     3082 2023-05-02 21:12:09.864720 bpkio_python_sdk-1.0.1/bpkio_api/helpers/profile_generator/hls.py
--rw-r--r--   0        0        0     1516 2023-05-02 21:16:30.728876 bpkio_python_sdk-1.0.1/bpkio_api/helpers/profile_generator/profile_generator.py
--rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.0.1/bpkio_api/helpers/search.py
--rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.0.1/bpkio_api/helpers/source_type.py
--rw-r--r--   0        0        0     2000 2023-05-12 19:28:37.449401 bpkio_python_sdk-1.0.1/bpkio_api/helpers/times.py
--rw-r--r--   0        0        0     2305 2023-05-04 09:38:29.832918 bpkio_python_sdk-1.0.1/bpkio_api/mappings.py
--rw-r--r--   0        0        0      305 2023-04-16 00:14:59.527618 bpkio_python_sdk-1.0.1/bpkio_api/models/Categories.py
--rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.0.1/bpkio_api/models/Consumption.py
--rw-r--r--   0        0        0     4498 2023-05-12 21:02:18.831085 bpkio_python_sdk-1.0.1/bpkio_api/models/Services.py
--rw-r--r--   0        0        0     1776 2023-04-27 17:11:34.397967 bpkio_python_sdk-1.0.1/bpkio_api/models/Slots.py
--rw-r--r--   0        0        0     3136 2023-05-01 20:17:25.667591 bpkio_python_sdk-1.0.1/bpkio_api/models/Sources.py
--rw-r--r--   0        0        0      413 2023-04-16 00:16:26.848163 bpkio_python_sdk-1.0.1/bpkio_api/models/Tenants.py
--rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.0.1/bpkio_api/models/TranscodingProfiles.py
--rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.0.1/bpkio_api/models/Users.py
--rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.0.1/bpkio_api/models/__init__.py
--rw-r--r--   0        0        0      911 2023-05-01 20:11:46.199279 bpkio_python_sdk-1.0.1/bpkio_api/models/common.py
--rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.0.1/bpkio_api/models/model_graph.py
--rw-r--r--   0        0        0     1604 2023-04-14 21:22:20.224021 bpkio_python_sdk-1.0.1/bpkio_api/response_handler.py
--rw-r--r--   0        0        0      860 2023-05-12 21:47:00.966751 bpkio_python_sdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.1.0/README.md
+-rw-r--r--   0        0        0      203 2023-05-17 14:14:39.237826 bpkio_python_sdk-1.1.0/bpkio_api/__init__.py
+-rw-r--r--   0        0        0     5127 2023-05-17 20:59:10.717567 bpkio_python_sdk-1.1.0/bpkio_api/api.py
+-rw-r--r--   0        0        0     1044 2023-04-20 16:56:18.119327 bpkio_python_sdk-1.1.0/bpkio_api/caching.py
+-rw-r--r--   0        0        0     4038 2023-05-17 21:43:51.682208 bpkio_python_sdk-1.1.0/bpkio_api/credential_provider.py
+-rw-r--r--   0        0        0       34 2023-04-30 20:15:10.400387 bpkio_python_sdk-1.1.0/bpkio_api/defaults.py
+-rw-r--r--   0        0        0      393 2023-04-07 16:54:49.526444 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/__init__.py
+-rw-r--r--   0        0        0     4379 2023-05-12 07:24:24.240126 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/categories.py
+-rw-r--r--   0        0        0      658 2023-04-14 21:22:20.218915 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/consumption.py
+-rw-r--r--   0        0        0    21801 2023-05-17 17:12:06.162415 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/services.py
+-rw-r--r--   0        0        0    21435 2023-05-16 19:15:10.787303 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/sources.py
+-rw-r--r--   0        0        0     2667 2023-05-12 07:24:24.242152 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/tenants.py
+-rw-r--r--   0        0        0     5713 2023-05-12 07:24:24.242673 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/transcoding_profiles.py
+-rw-r--r--   0        0        0     2619 2023-05-12 07:24:24.243027 bpkio_python_sdk-1.1.0/bpkio_api/endpoints/users.py
+-rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.1.0/bpkio_api/exceptions.py
+-rw-r--r--   0        0        0     2449 2023-04-29 21:37:29.834823 bpkio_python_sdk-1.1.0/bpkio_api/helpers/codecstrings.py
+-rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/__init__.py
+-rw-r--r--   0        0        0     4562 2023-05-05 10:37:16.925090 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/dash.py
+-rw-r--r--   0        0        0     3333 2023-05-04 10:23:23.525504 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/factory.py
+-rw-r--r--   0        0        0     1948 2023-05-02 20:36:39.412636 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/generic.py
+-rw-r--r--   0        0        0     4390 2023-05-17 17:41:42.490027 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/hls.py
+-rw-r--r--   0        0        0      436 2023-04-24 19:35:00.162089 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/jpeg.py
+-rw-r--r--   0        0        0      462 2023-04-24 19:37:38.335538 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/mp4.py
+-rw-r--r--   0        0        0      424 2023-04-24 19:36:40.587083 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/png.py
+-rw-r--r--   0        0        0     1956 2023-04-28 20:35:58.216707 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/vast.py
+-rw-r--r--   0        0        0     2305 2023-05-04 18:59:29.593036 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/vmap.py
+-rw-r--r--   0        0        0      560 2023-04-25 14:32:14.371116 bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/xml.py
+-rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.1.0/bpkio_api/helpers/list.py
+-rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.1.0/bpkio_api/helpers/objects.py
+-rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/__init__.py
+-rw-r--r--   0        0        0      461 2023-04-30 19:12:24.858790 bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/analyser.py
+-rw-r--r--   0        0        0     1713 2023-04-29 21:41:55.874476 bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/dash.py
+-rw-r--r--   0        0        0     3082 2023-05-02 21:12:09.864720 bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/hls.py
+-rw-r--r--   0        0        0     1516 2023-05-02 21:16:30.728876 bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/profile_generator.py
+-rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.1.0/bpkio_api/helpers/search.py
+-rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.1.0/bpkio_api/helpers/source_type.py
+-rw-r--r--   0        0        0     2000 2023-05-12 19:28:37.449401 bpkio_python_sdk-1.1.0/bpkio_api/helpers/times.py
+-rw-r--r--   0        0        0     2621 2023-05-17 14:38:59.521244 bpkio_python_sdk-1.1.0/bpkio_api/mappings.py
+-rw-r--r--   0        0        0      305 2023-04-16 00:14:59.527618 bpkio_python_sdk-1.1.0/bpkio_api/models/Categories.py
+-rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.1.0/bpkio_api/models/Consumption.py
+-rw-r--r--   0        0        0     4815 2023-05-16 12:12:43.320150 bpkio_python_sdk-1.1.0/bpkio_api/models/Services.py
+-rw-r--r--   0        0        0     1776 2023-04-27 17:11:34.397967 bpkio_python_sdk-1.1.0/bpkio_api/models/Slots.py
+-rw-r--r--   0        0        0     3136 2023-05-01 20:17:25.667591 bpkio_python_sdk-1.1.0/bpkio_api/models/Sources.py
+-rw-r--r--   0        0        0      413 2023-04-16 00:16:26.848163 bpkio_python_sdk-1.1.0/bpkio_api/models/Tenants.py
+-rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.1.0/bpkio_api/models/TranscodingProfiles.py
+-rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.1.0/bpkio_api/models/Users.py
+-rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.1.0/bpkio_api/models/__init__.py
+-rw-r--r--   0        0        0      911 2023-05-01 20:11:46.199279 bpkio_python_sdk-1.1.0/bpkio_api/models/common.py
+-rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.1.0/bpkio_api/models/model_graph.py
+-rw-r--r--   0        0        0     1604 2023-04-14 21:22:20.224021 bpkio_python_sdk-1.1.0/bpkio_api/response_handler.py
+-rw-r--r--   0        0        0     1195 2023-05-17 22:55:41.179720 bpkio_python_sdk-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.1.0/PKG-INFO
```

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/api.py` & `bpkio_python_sdk-1.1.0/bpkio_api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import os
 from typing import Optional
 
 from uplink import Consumer
 from uplink.auth import BearerToken
 
 from bpkio_api.caching import init_cache
-from bpkio_api.credential_provider import TenantProfileProvider
+from bpkio_api.credential_provider import TenantProfile, TenantProfileProvider
 from bpkio_api.defaults import DEFAULT_FQDN
 from bpkio_api.endpoints import (
     CategoriesApi,
     ConsumptionApi,
     ServicesApi,
     SourcesApi,
     TenantsApi,
     TranscodingProfilesApi,
     UsersApi,
 )
 from bpkio_api.exceptions import InvalidApiKeyFormat
+from bpkio_api.mappings import model_to_endpoint
 from bpkio_api.models import Tenant
 
 
 class BroadpeakIoApi(Consumer):
     def __init__(
         self,
         *,
@@ -34,15 +35,18 @@
     ):
         if tenant and api_key:
             raise ValueError("You can't specify both tenant and api_key")
 
         tp = TenantProfileProvider()
 
         if tenant:
-            t = tp.get_tenant_profile(tenant)
+            if isinstance(tenant, str):                
+                t = tp.get_tenant_profile(tenant)
+            if isinstance(tenant, TenantProfile):
+                t = tenant
             self._api_key = t.api_key
             self._fqdn = t.fqdn
 
         elif api_key:
             self._api_key = api_key
             self._fqdn = fqdn or DEFAULT_FQDN
 
@@ -144,7 +148,11 @@
         """Checks that the URL is a valid Broadpeak.io entrypoint"""
         try:
             api = BroadpeakIoApi(api_key=api_key, fqdn=url)
             api.get_self_tenant()
             return True
         except Exception as e:
             return False
+
+    def root_endpoint_for_resource(self, resource: object) -> object:
+        """Returns the root endpoint for a given resource"""
+        return model_to_endpoint(api=self, model=type(resource))
```

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/caching.py` & `bpkio_python_sdk-1.1.0/bpkio_api/caching.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/credential_provider.py` & `bpkio_python_sdk-1.1.0/bpkio_api/credential_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from bpkio_api.defaults import DEFAULT_FQDN
 
 DEFAULT_INI_FILE = path.join(path.expanduser("~"), ".bpkio/tenants")
 
 
 class TenantProfile(BaseModel):
     label: str
-    id: str
+    id: int
     fqdn: Optional[str] = DEFAULT_FQDN
     api_key: str
 
 
 class TenantProfileProvider:
     config = configparser.ConfigParser()
 
@@ -33,37 +33,49 @@
     def inifile(self):
         return self._filename
 
     def get_tenant_profile(self, tenant_label: str):
         return TenantProfile(
             label=tenant_label,
             api_key=self.config[tenant_label].get("api_key"),
-            id=self.config[tenant_label].get("id"),
+            id=self.config[tenant_label].getint("id"),
             fqdn=self.config[tenant_label].get("fqdn", DEFAULT_FQDN),
         )
 
     def list_tenants(self):
         tenants = []
         for section in self.config.sections():
             tenants.append(
                 TenantProfile(
                     label=section,
-                    id=self.config[section].get("id"),
+                    id=self.config[section].getint("id"),
                     fqdn=self.config[section].get("fqdn", DEFAULT_FQDN),
                     api_key=self.config[section].get("api_key"),
                 )
             )
         return tenants
 
     def has_tenant_label(self, tenant: str):
         return tenant in self.config
 
     def has_default_tenant(self):
         return self.has_tenant_label("default")
 
+    def get_admin_tenant(self, fqdn: str):
+        """Retrieves the admin tenant in the same stack as the current tenant,
+        if it is available in the `tenants` file.
+
+        Returns:
+            TenantProfile: The admin tenant.
+        """
+        for tenant in self.list_tenants():
+            if tenant.fqdn == fqdn and tenant.id == 1:
+                return tenant
+        return None
+
     # --- Core methods to read and write the `tenants` file ---
 
     def _get_tenant_section(self, tenant: str | None):
         tenant_section = None
         if tenant:
             if tenant in self.config:
                 # tenant is the key in a section of the config file
```

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/endpoints/categories.py` & `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/categories.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/endpoints/consumption.py` & `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/consumption.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/endpoints/services.py` & `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,24 @@
             parent_api=self, base_url=base_url, **kwargs
         )
 
     def _mappings(self, model):
         match model:
             case Svc.VirtualChannelServiceIn():
                 return self.virtual_channel
+            case Svc.VirtualChannelService():
+                return self.virtual_channel
             case Svc.AdInsertionServiceIn():
                 return self.ad_insertion
+            case Svc.AdInsertionService():
+                return self.ad_insertion
             case Svc.ContentReplacementServiceIn():
                 return self.content_replacement
+            case Svc.ContentReplacementService():
+                return self.content_replacement
             case _:
                 raise Exception(
                     f"Model {model.__class__.__name__} "
                     "not recognised as a valid service type"
                 )
 
     @returns.json(List[Svc.ServiceSparse])
@@ -154,14 +160,25 @@
         | Svc.ContentReplacementService
         | Svc.AdInsertionService
     ):
         """Create a service"""
         endpoint = self._mappings(service)
         return endpoint.create(service)
 
+    def delete(self, service_id: int):
+        """Delete a service"""
+        service = self.retrieve(service_id)
+        if not service:
+            raise BroadpeakIoHelperError(
+                status_code=404,
+                message=f"There is no service with ID {service_id}",
+            )
+        endpoint = self._mappings(service)
+        return endpoint.delete(service_id)
+
     def _update(
         self, service_id: int, service: Svc.ServiceIn
     ) -> (
         Svc.VirtualChannelService
         | Svc.ContentReplacementService
         | Svc.AdInsertionService
     ):
@@ -174,15 +191,15 @@
     ) -> (
         Svc.VirtualChannelService
         | Svc.ContentReplacementService
         | Svc.AdInsertionService
     ):
         """Create a service"""
         endpoint = self._mappings(service)
-        return endpoint.update(service)
+        return endpoint.update(service_id, service)
 
     def upsert(
         self,
         service: Svc.ServiceIn,
         if_exists: str = "retrieve",
         unique_fields: List[str | Tuple] = [],
     ) -> Tuple[
```

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/endpoints/sources.py` & `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,25 @@
         | S.SlateSource
         | S.LiveSource
     ):
         """Create a source"""
         endpoint = self._mappings(source)
         return endpoint.create(source)
 
+    def delete(self, source_id: int):
+        """Delete a source"""
+        source = self.retrieve(source_id)
+        if not source:
+            raise BroadpeakIoHelperError(
+                status_code=404,
+                message=f"There is no source with ID {source_id}",
+            )
+        endpoint = self._mappings(source)
+        return endpoint.delete(source_id)
+
     def _update(
         self, source_id: int, source: S.SourceIn
     ) -> (
         S.AssetSource
         | S.AdServerSource
         | S.AssetCatalogSource
         | S.SlateSource
```

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/endpoints/tenants.py` & `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/tenants.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/endpoints/transcoding_profiles.py` & `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/transcoding_profiles.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/endpoints/users.py` & `bpkio_python_sdk-1.1.0/bpkio_api/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/exceptions.py` & `bpkio_python_sdk-1.1.0/bpkio_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/codecstrings.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/codecstrings.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/dash.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/dash.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/factory.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/factory.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/generic.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/generic.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/hls.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/hls.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,17 +100,14 @@
             "type": "Live" if self.is_live() else "VOD",
             "duration (in sec)": "N/A" if self.is_live() else self.get_duration(),
             "segments": self.num_segments(),
         }
 
         return info
 
-    def extract_timeline(self):
-        pass
-
     def extract_features(self) -> List[Dict]:
         """Extracts essential information from the HLS manifest"""
         arr = []
         index = 0
 
         if self.document.is_variant:
             for playlist in self.document.playlists:
```

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/vast.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/vast.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/vmap.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/vmap.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/handlers/xml.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/handlers/xml.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/list.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/profile_generator/dash.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/dash.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/profile_generator/hls.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/hls.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/profile_generator/profile_generator.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/profile_generator/profile_generator.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/search.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/source_type.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/source_type.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/helpers/times.py` & `bpkio_python_sdk-1.1.0/bpkio_api/helpers/times.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/mappings.py` & `bpkio_python_sdk-1.1.0/bpkio_api/mappings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,16 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 import bpkio_api.models as m
-from bpkio_api.api import BroadpeakIoApi
+
+if TYPE_CHECKING:
+    from bpkio_api.api import BroadpeakIoApi
+    from bpkio_api.models.common import BaseResource
 
 
 def model_to_endpoint(api: BroadpeakIoApi, model: type):
     match model:
         case m.SourceSparse:
             return api.sources
         case m.AssetSource | m.AssetSourceIn:
@@ -52,9 +59,15 @@
     (m.Category, m.CategoryIn),
     (m.TranscodingProfile, m.TranscodingProfileIn),
     (m.ServiceSparse, m.ServiceIn),
     (m.SourceSparse, m.SourceIn),
 ]
 
 
-def model_to_model_in(model: type):
+def _model_to_input_model(model: type):
     return next(i for (o, i) in MODELS_OUT_IN if o == model)
+
+
+def to_input_model(resource: BaseResource):
+    in_model = _model_to_input_model(type(resource))
+    in_obj = in_model.parse_obj(resource.dict())
+    return in_obj
```

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/models/Services.py` & `bpkio_python_sdk-1.1.0/bpkio_api/models/Services.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,51 +104,62 @@
 
 class LiveAdPreRollModelIn(BaseModel):
     adServer: BaseResource
     maxDuration: Optional[float]
     offset: Optional[float]
 
 
-class AdInsertionServiceIn(ServiceIn):
-    vodAdInsertion: Optional[VodAdInsertionModelIn] = None
-    liveAdPreRoll: Optional[LiveAdPreRollModelIn] = None
-    liveAdReplacement: Optional[LiveAdReplacementModelIn] = None
-
-    # TODO: parse the specific sub-type of source
-    source: BaseResource
+class _WithCommonAdInsertionServiceFields:
     enableAdTranscoding: Optional[bool] = False
     enableServerSideAdTracking: Optional[bool] = False
     enableSSATCheckChunk: Optional[bool] = False
 
-    # TODO - migrate to TranscodingProfile Model
     transcodingProfile: Optional[TranscodingProfileId] = None
 
     @property
     def sub_type(self):
         for prop in ["vodAdInsertion", "liveAdPreRoll", "liveAdReplacement"]:
             if getattr(self, prop):
                 return prop
 
-
-class AdInsertionService(AdInsertionServiceIn, WithCommonServiceFields):
-    @property
-    def type(self):
-        return ServiceType.AD_INSERTION
-
     @property
     def full_url(self):
         return self.make_full_url()
 
     def make_full_url(self, extra=None, *args, **kwargs):
         if extra:
             return urljoin(self.url, extra)
 
         return self.url
 
 
+class AdInsertionServiceIn(ServiceIn, _WithCommonAdInsertionServiceFields):
+    vodAdInsertion: Optional[VodAdInsertionModelIn] = None
+    liveAdPreRoll: Optional[LiveAdPreRollModelIn] = None
+    liveAdReplacement: Optional[LiveAdReplacementModelIn] = None
+
+    # TODO: parse the specific sub-type of source
+    source: BaseResource
+
+
+class AdInsertionService(
+    ServiceIn, WithCommonServiceFields, _WithCommonAdInsertionServiceFields
+):
+    vodAdInsertion: Optional[VodAdInsertionModel] = None
+    liveAdPreRoll: Optional[LiveAdPreRollModel] = None
+    liveAdReplacement: Optional[LiveAdReplacementModel] = None
+
+    # TODO: parse the specific sub-type of source
+    source: SourceSparse
+
+    @property
+    def type(self):
+        return ServiceType.AD_INSERTION
+
+
 # === CONTENT-REPLACEMENT SERVICE Models ===
 
 
 class ContentReplacementServiceIn(ServiceIn):
     # TODO: parse the specific sub-type of source
     source: SourceSparse
     replacement: SourceSparse
```

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/models/Slots.py` & `bpkio_python_sdk-1.1.0/bpkio_api/models/Slots.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/models/Sources.py` & `bpkio_python_sdk-1.1.0/bpkio_api/models/Sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/models/__init__.py` & `bpkio_python_sdk-1.1.0/bpkio_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/models/common.py` & `bpkio_python_sdk-1.1.0/bpkio_api/models/common.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/models/model_graph.py` & `bpkio_python_sdk-1.1.0/bpkio_api/models/model_graph.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/bpkio_api/response_handler.py` & `bpkio_python_sdk-1.1.0/bpkio_api/response_handler.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.0.1/pyproject.toml` & `bpkio_python_sdk-1.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 [tool.poetry]
 name = "bpkio-python-sdk"
-version = "1.0.1"
+version = "1.1.0"
 description = "An (opinionated) Python SDK for the broadpeak.io REST APIs"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
-packages = [{include = "bpkio_api"}]
+packages = [{ include = "bpkio_api" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.10.7"
 uplink = "^0.9.7"
 setuptools = "^67.6.1"
 m3u8 = "^3.4.0"
 lxml = "^4.9.2"
 diskcache = "^5.4.0"
 mpd-parser = "^0.1.2"
 pymediainfo = "^6.0.1"
+pytz = "^2023.3"
 
+[tool.poetry-dynamic-versioning]
+enable = true
+vcs = "git"
+style = "semver"
+
+[tool.poetry-dynamic-versioning.substitution]
+files = ["*/__init__.py", "*/__version__.py", "*/_version.py"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.2"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 graphviz = "^0.20.1"
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 
+# [build-system]
+# requires = ["poetry-core"]
+# build-backend = "poetry.core.masonry.api"
+
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `bpkio_python_sdk-1.0.1/PKG-INFO` & `bpkio_python_sdk-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: bpkio-python-sdk
-Version: 1.0.1
+Version: 1.1.0
 Summary: An (opinionated) Python SDK for the broadpeak.io REST APIs
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: diskcache (>=5.4.0,<6.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: m3u8 (>=3.4.0,<4.0.0)
 Requires-Dist: mpd-parser (>=0.1.2,<0.2.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pymediainfo (>=6.0.1,<7.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: setuptools (>=67.6.1,<68.0.0)
 Requires-Dist: uplink (>=0.9.7,<0.10.0)
 Description-Content-Type: text/markdown
```

