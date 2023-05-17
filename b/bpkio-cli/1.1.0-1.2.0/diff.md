# Comparing `tmp/bpkio_cli-1.1.0.tar.gz` & `tmp/bpkio_cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_cli-1.1.0.tar", max compression
+gzip compressed data, was "bpkio_cli-1.2.0.tar", max compression
```

## Comparing `bpkio_cli-1.1.0.tar` & `bpkio_cli-1.2.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0        0 2023-03-28 20:04:37.409875 bpkio_cli-1.1.0/README.md
--rw-r--r--   0        0        0       22 2023-05-12 21:49:06.044277 bpkio_cli-1.1.0/bpkio_cli/__init__.py
--rw-r--r--   0        0        0     3338 2023-04-29 21:08:44.550102 bpkio_cli-1.1.0/bpkio_cli/__main__.py
--rw-r--r--   0        0        0       91 2023-04-29 21:05:12.410693 bpkio_cli-1.1.0/bpkio_cli/click_mods/__init__.py
--rw-r--r--   0        0        0     4511 2023-04-29 21:09:43.731932 bpkio_cli-1.1.0/bpkio_cli/click_mods/group_rest_resource.py
--rw-r--r--   0        0        0     1747 2023-03-23 13:12:03.515867 bpkio_cli-1.1.0/bpkio_cli/click_mods/option_eat_all.py
--rw-r--r--   0        0        0      564 2023-04-29 21:08:44.551140 bpkio_cli-1.1.0/bpkio_cli/commands/__init__.py
--rw-r--r--   0        0        0     4634 2023-05-12 21:43:26.529478 bpkio_cli-1.1.0/bpkio_cli/commands/configure.py
--rw-r--r--   0        0        0     1758 2023-04-28 08:13:42.029805 bpkio_cli-1.1.0/bpkio_cli/commands/consumption.py
--rw-r--r--   0        0        0      762 2023-04-26 12:03:04.836639 bpkio_cli-1.1.0/bpkio_cli/commands/hello.py
--rw-r--r--   0        0        0      983 2023-04-26 12:03:04.836946 bpkio_cli-1.1.0/bpkio_cli/commands/memory.py
--rw-r--r--   0        0        0     3134 2023-04-26 12:03:04.837256 bpkio_cli-1.1.0/bpkio_cli/commands/package.py
--rw-r--r--   0        0        0     6852 2023-05-12 19:43:30.439010 bpkio_cli-1.1.0/bpkio_cli/commands/profiles.py
--rw-r--r--   0        0        0     3401 2023-05-12 20:34:15.984115 bpkio_cli-1.1.0/bpkio_cli/commands/services.py
--rw-r--r--   0        0        0     3740 2023-05-12 21:34:14.672836 bpkio_cli-1.1.0/bpkio_cli/commands/services_create.py
--rw-r--r--   0        0        0     5419 2023-04-29 21:54:24.509681 bpkio_cli-1.1.0/bpkio_cli/commands/sources.py
--rw-r--r--   0        0        0    16787 2023-05-12 19:58:32.261329 bpkio_cli-1.1.0/bpkio_cli/commands/template_crud.py
--rw-r--r--   0        0        0     7223 2023-05-12 07:39:22.268209 bpkio_cli-1.1.0/bpkio_cli/commands/template_crud_slots.py
--rw-r--r--   0        0        0      332 2023-04-28 08:33:05.100937 bpkio_cli-1.1.0/bpkio_cli/commands/tenants.py
--rw-r--r--   0        0        0     5348 2023-05-12 07:40:30.476002 bpkio_cli-1.1.0/bpkio_cli/commands/url.py
--rw-r--r--   0        0        0      359 2023-04-28 08:33:22.939414 bpkio_cli-1.1.0/bpkio_cli/commands/users.py
--rw-r--r--   0        0        0     1043 2023-04-30 21:10:36.024729 bpkio_cli-1.1.0/bpkio_cli/core/app_settings.py
--rw-r--r--   0        0        0      135 2023-04-20 16:43:38.934392 bpkio_cli-1.1.0/bpkio_cli/core/exceptions.py
--rw-r--r--   0        0        0     2128 2023-04-30 21:09:27.517510 bpkio_cli-1.1.0/bpkio_cli/core/initialize.py
--rw-r--r--   0        0        0     1718 2023-04-07 16:07:08.180945 bpkio_cli-1.1.0/bpkio_cli/core/logger.py
--rw-r--r--   0        0        0     8665 2023-05-04 10:16:16.190924 bpkio_cli-1.1.0/bpkio_cli/core/packager.py
--rw-r--r--   0        0        0     5741 2023-04-29 21:14:44.072132 bpkio_cli-1.1.0/bpkio_cli/core/resource_recorder.py
--rw-r--r--   0        0        0     2207 2023-04-26 12:03:04.840592 bpkio_cli-1.1.0/bpkio_cli/core/resources_context.py
--rw-r--r--   0        0        0     5142 2023-05-12 18:56:36.153732 bpkio_cli-1.1.0/bpkio_cli/core/response_handler.py
--rw-r--r--   0        0        0      545 2023-05-12 07:26:04.407684 bpkio_cli-1.1.0/bpkio_cli/options/__init__.py
--rw-r--r--   0        0        0      304 2023-04-27 14:26:01.184020 bpkio_cli-1.1.0/bpkio_cli/options/admin.py
--rw-r--r--   0        0        0      355 2023-05-12 19:07:07.722647 bpkio_cli-1.1.0/bpkio_cli/options/json.py
--rw-r--r--   0        0        0      958 2023-05-12 07:26:58.744571 bpkio_cli-1.1.0/bpkio_cli/options/list.py
--rw-r--r--   0        0        0      933 2023-04-27 14:26:01.185185 bpkio_cli-1.1.0/bpkio_cli/options/poll.py
--rw-r--r--   0        0        0      568 2023-05-02 19:55:34.650018 bpkio_cli-1.1.0/bpkio_cli/options/read.py
--rw-r--r--   0        0        0     1183 2023-04-27 14:26:01.185667 bpkio_cli-1.1.0/bpkio_cli/options/search.py
--rw-r--r--   0        0        0      445 2023-05-04 18:13:29.662132 bpkio_cli-1.1.0/bpkio_cli/options/table.py
--rw-r--r--   0        0        0      777 2023-05-04 11:31:15.973002 bpkio_cli-1.1.0/bpkio_cli/options/urls.py
--rw-r--r--   0        0        0      289 2023-05-12 07:26:12.169733 bpkio_cli-1.1.0/bpkio_cli/utils/__init__.py
--rw-r--r--   0        0        0     2288 2023-05-12 07:34:26.643986 bpkio_cli-1.1.0/bpkio_cli/utils/arrays.py
--rw-r--r--   0        0        0     3398 2023-05-12 19:50:24.682253 bpkio_cli-1.1.0/bpkio_cli/utils/config_provider.py
--rw-r--r--   0        0        0     1202 2023-04-28 08:03:11.236380 bpkio_cli-1.1.0/bpkio_cli/utils/datetimes.py
--rw-r--r--   0        0        0      136 2023-04-14 20:15:18.159888 bpkio_cli-1.1.0/bpkio_cli/utils/json.py
--rw-r--r--   0        0        0      567 2023-04-29 21:58:38.435162 bpkio_cli-1.1.0/bpkio_cli/utils/profile_maker.py
--rw-r--r--   0        0        0     4658 2023-05-12 19:12:42.208834 bpkio_cli-1.1.0/bpkio_cli/utils/url_builders.py
--rw-r--r--   0        0        0      583 2023-04-09 19:02:06.960542 bpkio_cli-1.1.0/bpkio_cli/utils/urls.py
--rw-r--r--   0        0        0      611 2023-04-21 22:26:37.261644 bpkio_cli-1.1.0/bpkio_cli/writers/breadcrumbs.py
--rw-r--r--   0        0        0     1404 2023-05-02 20:19:18.033992 bpkio_cli-1.1.0/bpkio_cli/writers/colorizer.py
--rw-r--r--   0        0        0     4128 2023-05-02 20:54:33.828754 bpkio_cli-1.1.0/bpkio_cli/writers/content_display.py
--rw-r--r--   0        0        0      840 2023-04-26 12:03:04.848088 bpkio_cli-1.1.0/bpkio_cli/writers/diff.py
--rw-r--r--   0        0        0      152 2023-04-26 12:03:04.848777 bpkio_cli-1.1.0/bpkio_cli/writers/formatter.py
--rw-r--r--   0        0        0     4533 2023-05-09 10:21:54.315733 bpkio_cli-1.1.0/bpkio_cli/writers/hls_formatter.py
--rw-r--r--   0        0        0      715 2023-05-12 19:01:29.004428 bpkio_cli-1.1.0/bpkio_cli/writers/json_formatter.py
--rw-r--r--   0        0        0     1583 2023-04-29 21:08:44.553756 bpkio_cli-1.1.0/bpkio_cli/writers/players.py
--rw-r--r--   0        0        0     1865 2023-05-12 07:26:12.170387 bpkio_cli-1.1.0/bpkio_cli/writers/tables.py
--rw-r--r--   0        0        0     5205 2023-04-26 12:03:04.849885 bpkio_cli-1.1.0/bpkio_cli/writers/xml_formatter.py
--rw-r--r--   0        0        0     1209 2023-05-12 21:55:00.912742 bpkio_cli-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 bpkio_cli-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-28 20:04:37.409875 bpkio_cli-1.2.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-17 22:57:42.076244 bpkio_cli-1.2.0/bpkio_cli/__init__.py
+-rw-r--r--   0        0        0     3338 2023-04-29 21:08:44.550102 bpkio_cli-1.2.0/bpkio_cli/__main__.py
+-rw-r--r--   0        0        0       91 2023-04-29 21:05:12.410693 bpkio_cli-1.2.0/bpkio_cli/click_mods/__init__.py
+-rw-r--r--   0        0        0     4511 2023-05-16 18:51:59.357188 bpkio_cli-1.2.0/bpkio_cli/click_mods/group_rest_resource.py
+-rw-r--r--   0        0        0     1747 2023-03-23 13:12:03.515867 bpkio_cli-1.2.0/bpkio_cli/click_mods/option_eat_all.py
+-rw-r--r--   0        0        0      564 2023-04-29 21:08:44.551140 bpkio_cli-1.2.0/bpkio_cli/commands/__init__.py
+-rw-r--r--   0        0        0     4669 2023-05-17 17:39:31.235348 bpkio_cli-1.2.0/bpkio_cli/commands/configure.py
+-rw-r--r--   0        0        0     1758 2023-04-28 08:13:42.029805 bpkio_cli-1.2.0/bpkio_cli/commands/consumption.py
+-rw-r--r--   0        0        0      762 2023-04-26 12:03:04.836639 bpkio_cli-1.2.0/bpkio_cli/commands/hello.py
+-rw-r--r--   0        0        0      983 2023-04-26 12:03:04.836946 bpkio_cli-1.2.0/bpkio_cli/commands/memory.py
+-rw-r--r--   0        0        0     3134 2023-04-26 12:03:04.837256 bpkio_cli-1.2.0/bpkio_cli/commands/package.py
+-rw-r--r--   0        0        0     8349 2023-05-17 22:14:59.854931 bpkio_cli-1.2.0/bpkio_cli/commands/profiles.py
+-rw-r--r--   0        0        0     3329 2023-05-16 18:56:25.674679 bpkio_cli-1.2.0/bpkio_cli/commands/services.py
+-rw-r--r--   0        0        0     3714 2023-05-12 22:00:13.183439 bpkio_cli-1.2.0/bpkio_cli/commands/services_create.py
+-rw-r--r--   0        0        0     5411 2023-05-16 18:54:19.088895 bpkio_cli-1.2.0/bpkio_cli/commands/sources.py
+-rw-r--r--   0        0        0    17617 2023-05-17 17:37:14.203105 bpkio_cli-1.2.0/bpkio_cli/commands/template_crud.py
+-rw-r--r--   0        0        0     7223 2023-05-12 07:39:22.268209 bpkio_cli-1.2.0/bpkio_cli/commands/template_crud_slots.py
+-rw-r--r--   0        0        0      332 2023-04-28 08:33:05.100937 bpkio_cli-1.2.0/bpkio_cli/commands/tenants.py
+-rw-r--r--   0        0        0     5348 2023-05-12 07:40:30.476002 bpkio_cli-1.2.0/bpkio_cli/commands/url.py
+-rw-r--r--   0        0        0      359 2023-04-28 08:33:22.939414 bpkio_cli-1.2.0/bpkio_cli/commands/users.py
+-rw-r--r--   0        0        0     1043 2023-04-30 21:10:36.024729 bpkio_cli-1.2.0/bpkio_cli/core/app_settings.py
+-rw-r--r--   0        0        0      135 2023-04-20 16:43:38.934392 bpkio_cli-1.2.0/bpkio_cli/core/exceptions.py
+-rw-r--r--   0        0        0     2128 2023-04-30 21:09:27.517510 bpkio_cli-1.2.0/bpkio_cli/core/initialize.py
+-rw-r--r--   0        0        0     1718 2023-04-07 16:07:08.180945 bpkio_cli-1.2.0/bpkio_cli/core/logger.py
+-rw-r--r--   0        0        0     8594 2023-05-17 14:18:10.837863 bpkio_cli-1.2.0/bpkio_cli/core/packager.py
+-rw-r--r--   0        0        0     5767 2023-05-16 18:56:45.783044 bpkio_cli-1.2.0/bpkio_cli/core/resource_recorder.py
+-rw-r--r--   0        0        0     2207 2023-04-26 12:03:04.840592 bpkio_cli-1.2.0/bpkio_cli/core/resources_context.py
+-rw-r--r--   0        0        0     5128 2023-05-16 19:08:30.137349 bpkio_cli-1.2.0/bpkio_cli/core/response_handler.py
+-rw-r--r--   0        0        0      545 2023-05-12 07:26:04.407684 bpkio_cli-1.2.0/bpkio_cli/options/__init__.py
+-rw-r--r--   0        0        0      848 2023-05-17 22:07:10.594805 bpkio_cli-1.2.0/bpkio_cli/options/admin.py
+-rw-r--r--   0        0        0      355 2023-05-12 19:07:07.722647 bpkio_cli-1.2.0/bpkio_cli/options/json.py
+-rw-r--r--   0        0        0      958 2023-05-12 07:26:58.744571 bpkio_cli-1.2.0/bpkio_cli/options/list.py
+-rw-r--r--   0        0        0      933 2023-04-27 14:26:01.185185 bpkio_cli-1.2.0/bpkio_cli/options/poll.py
+-rw-r--r--   0        0        0      568 2023-05-02 19:55:34.650018 bpkio_cli-1.2.0/bpkio_cli/options/read.py
+-rw-r--r--   0        0        0     1183 2023-04-27 14:26:01.185667 bpkio_cli-1.2.0/bpkio_cli/options/search.py
+-rw-r--r--   0        0        0      445 2023-05-04 18:13:29.662132 bpkio_cli-1.2.0/bpkio_cli/options/table.py
+-rw-r--r--   0        0        0      777 2023-05-04 11:31:15.973002 bpkio_cli-1.2.0/bpkio_cli/options/urls.py
+-rw-r--r--   0        0        0      396 2023-05-17 16:16:32.031925 bpkio_cli-1.2.0/bpkio_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2288 2023-05-12 07:34:26.643986 bpkio_cli-1.2.0/bpkio_cli/utils/arrays.py
+-rw-r--r--   0        0        0     3398 2023-05-12 19:50:24.682253 bpkio_cli-1.2.0/bpkio_cli/utils/config_provider.py
+-rw-r--r--   0        0        0     1202 2023-04-28 08:03:11.236380 bpkio_cli-1.2.0/bpkio_cli/utils/datetimes.py
+-rw-r--r--   0        0        0     1829 2023-05-17 22:20:51.013190 bpkio_cli-1.2.0/bpkio_cli/utils/editor.py
+-rw-r--r--   0        0        0      136 2023-04-14 20:15:18.159888 bpkio_cli-1.2.0/bpkio_cli/utils/json.py
+-rw-r--r--   0        0        0      567 2023-04-29 21:58:38.435162 bpkio_cli-1.2.0/bpkio_cli/utils/profile_maker.py
+-rw-r--r--   0        0        0     4658 2023-05-12 19:12:42.208834 bpkio_cli-1.2.0/bpkio_cli/utils/url_builders.py
+-rw-r--r--   0        0        0      583 2023-04-09 19:02:06.960542 bpkio_cli-1.2.0/bpkio_cli/utils/urls.py
+-rw-r--r--   0        0        0      611 2023-04-21 22:26:37.261644 bpkio_cli-1.2.0/bpkio_cli/writers/breadcrumbs.py
+-rw-r--r--   0        0        0     1404 2023-05-02 20:19:18.033992 bpkio_cli-1.2.0/bpkio_cli/writers/colorizer.py
+-rw-r--r--   0        0        0     4128 2023-05-02 20:54:33.828754 bpkio_cli-1.2.0/bpkio_cli/writers/content_display.py
+-rw-r--r--   0        0        0      840 2023-04-26 12:03:04.848088 bpkio_cli-1.2.0/bpkio_cli/writers/diff.py
+-rw-r--r--   0        0        0      152 2023-04-26 12:03:04.848777 bpkio_cli-1.2.0/bpkio_cli/writers/formatter.py
+-rw-r--r--   0        0        0     4533 2023-05-09 10:21:54.315733 bpkio_cli-1.2.0/bpkio_cli/writers/hls_formatter.py
+-rw-r--r--   0        0        0      715 2023-05-12 19:01:29.004428 bpkio_cli-1.2.0/bpkio_cli/writers/json_formatter.py
+-rw-r--r--   0        0        0     1583 2023-04-29 21:08:44.553756 bpkio_cli-1.2.0/bpkio_cli/writers/players.py
+-rw-r--r--   0        0        0     1865 2023-05-12 07:26:12.170387 bpkio_cli-1.2.0/bpkio_cli/writers/tables.py
+-rw-r--r--   0        0        0     5205 2023-04-26 12:03:04.849885 bpkio_cli-1.2.0/bpkio_cli/writers/xml_formatter.py
+-rw-r--r--   0        0        0     1207 2023-05-17 22:57:42.075576 bpkio_cli-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 bpkio_cli-1.2.0/PKG-INFO
```

### Comparing `bpkio_cli-1.1.0/bpkio_cli/__main__.py` & `bpkio_cli-1.2.0/bpkio_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/click_mods/group_rest_resource.py` & `bpkio_cli-1.2.0/bpkio_cli/click_mods/group_rest_resource.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/click_mods/option_eat_all.py` & `bpkio_cli-1.2.0/bpkio_cli/click_mods/option_eat_all.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/__init__.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/configure.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,18 @@
 @click.argument("tenant", required=False)
 @click.pass_context
 def switch(ctx, tenant):
     if not tenant:
         cp = TenantProfileProvider()
         tenant_list = cp.list_tenants()
         tenant_list = sorted(tenant_list, key=lambda t: t.label)
-        choices = [dict(value=t.label, name=f"{t.label} ({t.id})  -  {t.fqdn}") for t in tenant_list]
+        choices = [
+            dict(value=t.label, name=f"{t.label} ({t.id})  -  {t.fqdn}")
+            for t in tenant_list
+        ]
 
         tenant = inquirer.fuzzy(message="Select a tenant", choices=choices).execute()
 
     # Write it to the .tenant file
     with open(".tenant", "w") as f:
         f.write(tenant)
 
@@ -149,8 +152,9 @@
         )
 
 
 # Command: EDIT
 @tenants.command(help="Edit the tenant credential file manually")
 def edit():
     cp = TenantProfileProvider()
+
     click.edit(filename=str(cp.inifile), editor=ConfigProvider().get("editor"))
```

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/consumption.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/consumption.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/hello.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/hello.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/memory.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/memory.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/package.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/package.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/profiles.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/profiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,59 @@
 import json as j
 
 import click
 import cloup
+from bpkio_api.api import BroadpeakIoApi
 from bpkio_api.models import TranscodingProfile, TranscodingProfileIn
 from InquirerPy import inquirer
 
 import bpkio_cli.options as bic_options
 from bpkio_cli.click_mods import ApiResourceGroup
 from bpkio_cli.core.app_settings import AppContext
+from bpkio_cli.core.exceptions import BroadpeakIoCliError
 from bpkio_cli.utils.arrays import order_by_dict_keys
-from bpkio_cli.utils.config_provider import ConfigProvider
+from bpkio_cli.utils.editor import edit_payload
 from bpkio_cli.utils.json import is_json
 from bpkio_cli.writers.breadcrumbs import display_resource_info
 from bpkio_cli.writers.tables import display_table
 
 default_fields = ["id", "name", "num_layers"]
 
 
+def get_profile_skeleton():
+    return {
+        "packaging": {},
+        "servicetype": "offline_transcoding",
+        "transcoding": {
+            "jobs": [],
+            "common": {},
+        },
+    }
+
+
+def get_admin_endpoint():
+    ctx = click.get_current_context()
+    if ctx.obj.tenant.id == 1:
+        return ctx.obj.api.transcoding_profiles
+    else:
+        admin_tenant = ctx.obj.tenant_provider.get_admin_tenant(fqdn=ctx.obj.api.fqdn)
+        if not admin_tenant:
+            raise BroadpeakIoCliError(
+                "Admin tenant not found. You can only create profiles if you have admin rights"
+            )
+        admin_api = BroadpeakIoApi(tenant=admin_tenant)
+        return admin_api.transcoding_profiles
+
+
+def get_profile_resource(tenant=None):
+    ctx = click.get_current_context()
+    id = ctx.obj.resources.last()
+    return ctx.obj.api.transcoding_profiles.retrieve(id, tenantId=tenant)
+
+
 # # --- TRANSCODING PROFILES Group
 @cloup.group(
     cls=ApiResourceGroup,
     aliases=["prf", "profiles", "transcoding-profile"],
     show_subcommand_aliases=True,
     resource_class=TranscodingProfile,
 )
@@ -41,15 +74,15 @@
         display_resource_info(profile)
 
 
 # --- LIST Command
 @cloup.command(help="Retrieve a list of all Transcoding Profiles", aliases=["ls"])
 @bic_options.json
 @bic_options.list(default_fields=default_fields)
-@bic_options.tenant
+@bic_options.tenant(required=False)
 @click.pass_obj
 def list(obj, json, select_fields, sort_fields, tenant):
     profiles = obj.api.transcoding_profiles.list(tenantId=tenant)
 
     obj.response_handler.treat_list_resources(
         profiles,
         select_fields=select_fields,
@@ -66,38 +99,36 @@
 @click.option(
     "--table/--no-table",
     "with_table",
     is_flag=True,
     default=True,
     help="Add or hide summary information about the content of the resource",
 )
-@bic_options.tenant
+@bic_options.tenant(required=False)
 @bic_options.json
 @click.pass_context
 def get(ctx, tenant, json, with_table):
-    id = ctx.obj.resources.last()
-    profile = ctx.obj.api.transcoding_profiles.retrieve(id, tenantId=tenant)
+    profile = get_profile_resource(tenant)
 
     ctx.obj.response_handler.treat_single_resource(profile, json=json)
 
     if with_table and not json:
         ctx.invoke(table, header=False)
 
 
 # --- TABLE Command
 @cloup.command(help="Provide summary table of the content of the profile")
-@bic_options.tenant
+@bic_options.tenant(required=False)
 @click.pass_obj
 def table(
     obj: AppContext,
     tenant,
     **kwargs,
 ):
-    id = obj.resources.last()
-    profile = obj.api.transcoding_profiles.retrieve(id, tenantId=tenant)
+    profile = get_profile_resource(tenant)
     common = {
         k: click.style(v, dim=True)
         for k, v in profile.json_content["transcoding"]["common"].items()
     }
     jobs = [dict(common, **job) for job in profile.json_content["transcoding"]["jobs"]]
     jobs = order_by_dict_keys(jobs)
 
@@ -106,35 +137,35 @@
 
 # --- JSON Command
 @cloup.command(
     help="Get the JSON representation of a single Transcoding Profile "
     "or list of Transcoding Profiles"
 )
 @click.option(
-    "-e",
-    "--expand",
+    "-c",
+    "--content",
+    "content_only",
     is_flag=True,
     default=False,
     help="Extract the actual profile's JSON and pretty print it",
 )
-@bic_options.tenant
+@bic_options.tenant(required=False)
 @click.pass_obj
-def json(obj: AppContext, tenant, expand):
+def json(obj: AppContext, tenant, content_only):
     try:
-        id = obj.resources.last()
-        profile = obj.api.transcoding_profiles.retrieve(id, tenantId=tenant)
+        profile = get_profile_resource(tenant)
 
-        if expand:
+        if content_only:
             profile = profile.json_content
 
         obj.response_handler.treat_single_resource(profile, json=True)
 
     except Exception:
         profiles = obj.api.transcoding_profiles.list(tenantId=tenant)
-        if expand:
+        if content_only:
             # TODO - Dirty code. Needs resolving, maybe at level of the SDK
             bare_profiles = []
             for profile in profiles:
                 new_pro = j.loads(profile.json())
                 new_pro["_expanded_content"] = profile.json_content
                 bare_profiles.append(new_pro)
             profiles = bare_profiles
@@ -149,15 +180,15 @@
 @cloup.command(
     help="Retrieve a list of all Transcoding Profiles that match given "
     "terms in all or selected fields"
 )
 @bic_options.search
 @bic_options.json
 @bic_options.list(default_fields=default_fields)
-@bic_options.tenant
+@bic_options.tenant(required=False)
 @click.pass_obj
 def search(
     obj,
     tenant,
     single_term,
     search_terms,
     search_fields,
@@ -175,63 +206,84 @@
         sort_fields=sort_fields,
         json=json,
     )
 
 
 # --- CREATE Command
 @cloup.command(help="[ADMIN] Create a Transcoding Profile")
-@bic_options.tenant
+@bic_options.tenant(required=True)
 @cloup.option("--from", "from_file", type=click.File("r"), required=False, default=None)
 @cloup.option("--name", type=str, required=False, default=None)
 @click.pass_obj
 def create(obj: AppContext, tenant: int, from_file, name: str):
+    # set the correct context to create the API
+    endpoint = get_admin_endpoint()
+
+    # get the content of the profile
     if from_file:
-        content = from_file.read()
+        content = j.loads(from_file.read())
     else:
-        content = inquirer.text(
-            message="Content of the profile: ",
-            multiline=True,
-            validate=lambda txt: is_json(txt),
-            invalid_message="This is not a valid JSON payload",
-        ).execute()
+        content = get_profile_skeleton()
+
+    payload = edit_payload(content, is_json=True)
+    if not is_json(payload):
+        raise ValueError("The content of the profile is not valid JSON")
 
     if not name:
         name = inquirer.text(message="Name: ").execute()
 
-    tpro = TranscodingProfileIn(content=content, name=name, tenantId=None)
+    # build the profile object for creation
+    tpro = TranscodingProfileIn(content=payload, name=name, tenantId=None)
     if tenant:
         tpro.tenantId = tenant
 
-    out_profile = obj.api.transcoding_profiles.create(profile=tpro)
+    out_profile = endpoint.create(profile=tpro)
     obj.response_handler.treat_single_resource(out_profile)
 
 
 # --- UPDATE Command
-@cloup.command(aliases=["put"], help="Update a Transcoding Profile")
-@bic_options.tenant
+@cloup.command(aliases=["put"], help="[ADMIN] Update a Transcoding Profile")
+@click.option(
+    "-c",
+    "--content",
+    "content_only",
+    is_flag=True,
+    default=False,
+    help="Update the content of the profile, as a JSON payload",
+)
+@bic_options.tenant(required=True)
 @click.pass_obj
-def update(obj: AppContext, tenant: int):
-    id = obj.resources.last()
-    profile = obj.api.transcoding_profiles.retrieve(id, tenantId=tenant)
+def update(obj: AppContext, tenant: int, content_only: bool):
+    profile = get_profile_resource(tenant)
     profile.tenantId = tenant
-    payload = j.dumps(j.loads(profile.json()), indent=2)
 
-    updated_resource_json = click.edit(payload, editor=ConfigProvider().get("editor"))
+    if content_only:
+        edited_content = edit_payload(profile.json_content, is_json=True)
+        edited_profile = profile
+        profile.content = edited_content
+    else:
+        edited_profile = edit_payload(profile, is_json=True)
 
-    obj.api.transcoding_profiles.update(id, j.loads(updated_resource_json))
+    endpoint = get_admin_endpoint()
+    edited_profile = endpoint.update(profile.id, edited_profile)
 
-    click.secho(f"Resource {id} updated", fg="green")
+    click.secho(f"Resource {profile.id} updated", fg="green")
+    obj.response_handler.treat_single_resource(edited_profile)
 
 
 # --- DELETE Command
 @cloup.command(help="[ADMIN] Delete a Transcoding Profile, by its ID")
-@click.pass_obj
-def delete(obj: AppContext):
-    id = obj.resources.last()
-    obj.api.transcoding_profiles.delete(id)
+@click.confirmation_option(
+    prompt="Are you sure you want to delete this transcoding profile?"
+)
+def delete():
+    profile = get_profile_resource()
+    endpoint = get_admin_endpoint()
+
+    endpoint.delete(profile.id)
 
 
 profile.add_section(
     cloup.Section(
         "CRUD commands", [list, get, table, json, search, create, update, delete]
     )
 )
```

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/services.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/services.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-import click
 import cloup
 from bpkio_api.models import (
     AdInsertionService,
     ContentReplacementService,
     ContentReplacementSlot,
-    ServiceSparse,
+    ServiceIn,
     VirtualChannelService,
     VirtualChannelSlot,
 )
-from bpkio_cli.commands.services_create import create_ad_insertion_service_command
 
+from bpkio_cli.commands.services_create import create_ad_insertion_service_command
 from bpkio_cli.commands.template_crud import create_resource_group
 from bpkio_cli.commands.template_crud_slots import create_child_resource_group
-from bpkio_cli.core.app_settings import AppContext
 
 default_fields = ["id", "name", "type", "serviceId", "format"]
 
 
 def add_services_section(cli):
     root_endpoint = "services"
     root: cloup.Group = create_resource_group(
         "service",
-        resource_class=ServiceSparse,
+        resource_class=ServiceIn,
         endpoint_path=[root_endpoint],
         aliases=["svc", "services"],
         with_content_commands=["all"],
         default_fields=default_fields,
     )
 
     return cli.section(
@@ -57,15 +55,15 @@
         create_resource_group(
             "ad-insertion",
             resource_class=AdInsertionService,
             endpoint_path=[root_endpoint, "ad_insertion"],
             aliases=["dai", "ssai"],
             default_fields=["id", "name", "type", "sub_type", "serviceId", "format"],
             with_content_commands=["all"],
-            extra_commands=[create_ad_insertion_service_command()]
+            extra_commands=[create_ad_insertion_service_command()],
         ),
         create_resource_group(
             "virtual-channel",
             resource_class=VirtualChannelService,
             endpoint_path=[root_endpoint, "virtual_channel"],
             aliases=["vc"],
             default_fields=default_fields,
@@ -94,8 +92,7 @@
     return create_child_resource_group(
         "slot",
         resource_class=resource_class,
         endpoint_path=parent_path + ["slots"],
         aliases=["slots"],
         default_fields=default_fields,
     )
-
```

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/services_create.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/services_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def create(obj: AppContext):
         all_sources = obj.api.sources.list()
 
         # Ask for the source
         sources = [
             s
             for s in all_sources
-            if s.type in (SourceType.LIVE, SourceType.ASSET, SourceType.ASSET_CATALOG)
+            if s.type in (SourceType.LIVE, SourceType.ASSET_CATALOG)
         ]
         sources = sorted(sources, key=lambda s: s.id, reverse=True)
         choices = [
             dict(value=s.id, name=f"({s.id})  {s.name}  [{s.type.value}]")
             for s in sources
         ]
         source_id = inquirer.fuzzy(message="Source", choices=choices).execute()
@@ -77,15 +77,15 @@
         # Create the service object
         service = AdInsertionServiceIn(
             name=name, source=dict(id=source_id), enableAdTranscoding=with_transcoding
         )
         ad_insertion = dict(adServer=dict(id=ad_source_id))
         if slate_source_id is not None:
             ad_insertion["gapFiller"] = dict(id=slate_source_id)
-        
+
         setattr(
             service,
             insertion_type,
             ad_insertion,
         )
         if with_transcoding:
             service.transcodingProfile = dict(id=transcoding_profile_id)
```

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/sources.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     AssetCatalogSourceIn,
     AssetSource,
     AssetSourceIn,
     LiveSource,
     LiveSourceIn,
     SlateSource,
     SlateSourceIn,
-    SourceSparse,
+    SourceIn,
     SourceType,
 )
 from InquirerPy import inquirer
 from InquirerPy.base.control import Choice
 
 from bpkio_cli.commands.template_crud import create_resource_group
 from bpkio_cli.core.app_settings import AppContext
@@ -102,15 +102,15 @@
     obj.response_handler.treat_single_resource(source)
 
 
 def add_sources_section(cli):
     root_endpoint = "sources"
     root: cloup.Group = create_resource_group(
         "source",
-        resource_class=SourceSparse,
+        resource_class=SourceIn,
         endpoint_path=[root_endpoint],
         aliases=["src", "sources"],
         with_content_commands=["all"],
         default_fields=["id", "name", "type", "format", "url"],
     )
 
     root.add_command(create)
```

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/template_crud.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/template_crud.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import json as j
 import re
 from typing import List
 from urllib.parse import quote_plus
 
+import bpkio_api.mappings as mappings
 import click
 import cloup
 from bpkio_api.models import ServiceIn, SourceIn
 
 import bpkio_cli.options as bic_options
 from bpkio_cli.click_mods.group_rest_resource import ApiResourceGroup
 from bpkio_cli.commands.package import package_resources
 from bpkio_cli.core.app_settings import AppContext
 from bpkio_cli.core.exceptions import BroadpeakIoCliError
 from bpkio_cli.core.resources_context import ResourcesContext, UnknownResourceError
-from bpkio_cli.utils.config_provider import ConfigProvider
+from bpkio_cli.utils.editor import edit_payload
 from bpkio_cli.utils.profile_maker import make_transcoding_profile
 from bpkio_cli.utils.url_builders import get_service_handler, get_source_handler
 from bpkio_cli.writers.breadcrumbs import display_resource_info
 from bpkio_cli.writers.content_display import display_content
 from bpkio_cli.writers.players import StreamPlayer
 from bpkio_cli.writers.tables import display_table
 
@@ -61,19 +61,26 @@
         api = click.get_current_context().obj.api
         endpoint = api
         for p in path:
             endpoint = getattr(endpoint, p)
         return endpoint
 
     def retrieve_resource(id: int | str | None = None):
-        resource_context: ResourcesContext = click.get_current_context().obj.resources
+        ctx = click.get_current_context()
+        resource_context: ResourcesContext = ctx.obj.resources
         if not id:
             id = resource_context.last()
         endpoint = get_api_endpoint()
-        return endpoint.retrieve(id)
+        resource = endpoint.retrieve(id)
+
+        # Record the resource
+        if ctx.obj.cache and hasattr(resource, "id"):
+            ctx.obj.cache.record(resource)
+
+        return resource
 
     def get_content_handler(
         resource, replacement_fqdn=None, extra_url=None, subplaylist_index=None
     ):
         api = click.get_current_context().obj.api
 
         if isinstance(resource, SourceIn):
@@ -213,28 +220,53 @@
         click.secho(f"Resource {resource.id} deleted", fg="green")
 
     # --- UPDATE Command
     @cloup.command(aliases=["put"], help=f"Update a {resource_title}")
     @click.pass_context
     def update(ctx):
         resource = retrieve_resource()
-        payload = j.dumps(j.loads(resource.json()), indent=2)
 
-        updated_resource_json = click.edit(
-            payload, editor=ConfigProvider().get("editor")
-        )
+        updated_resource = edit_payload(resource)
 
         endpoint = get_api_endpoint()
         # TODO - try to parse into the resource class (otherwise can only work with specific resource sub-types)
-        endpoint.update(resource.id, j.loads(updated_resource_json))
+        endpoint.update(resource.id, updated_resource)
 
         click.secho(f"Resource {resource.id} updated", fg="green")
 
+    # --- DUPLICATE Command
+    @cloup.command(aliases=["copy"], help=f"Duplicate a {resource_title}")
+    @click.option(
+        "-e",
+        "--edit",
+        help="Edit the duplicated resource before saving it",
+        is_flag=True,
+        default=False,
+    )
+    @click.pass_obj
+    def duplicate(obj, edit):
+        resource = retrieve_resource()
+        endpoint = obj.api.root_endpoint_for_resource(resource)
+
+        resource.name = resource.name + " (copy)"
+
+        # remap to an input model
+        resource = mappings.to_input_model(resource)
+
+        if edit:
+            resource = edit_payload(resource)
+
+        new_resource = endpoint.create(resource)
+
+        obj.response_handler.treat_single_resource(new_resource, json=True)
+
     sections.append(
-        cloup.Section("CRUD commands", [list, get, json, search, delete, update])
+        cloup.Section(
+            "CRUD commands", [list, get, json, search, delete, update, duplicate]
+        )
     )
 
     # === CONTENT Commands ===
 
     content_section = cloup.Section("Content commands", [])
 
     if any(x in with_content_commands for x in ["all", "url"]):
```

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/template_crud_slots.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/template_crud_slots.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/commands/url.py` & `bpkio_cli-1.2.0/bpkio_cli/commands/url.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/core/app_settings.py` & `bpkio_cli-1.2.0/bpkio_cli/core/app_settings.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/core/initialize.py` & `bpkio_cli-1.2.0/bpkio_cli/core/initialize.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/core/logger.py` & `bpkio_cli-1.2.0/bpkio_cli/core/logger.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/core/packager.py` & `bpkio_cli-1.2.0/bpkio_cli/core/packager.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,26 +115,25 @@
             orig_id = resource.id
 
             # Create a GUID to replace it with
             guid = str(uuid.uuid4())
             self.id_mappings[orig_id] = guid
 
             # Transform the resource into an IN model
-            in_model: BaseModel = mappings.model_to_model_in(type(resource))
-            in_obj = in_model.parse_obj(resource.dict())
+            in_obj = mappings.to_input_model(resource)
 
             # Replace dependent IDs in it
             replace_guid_with_id(in_obj)
 
             # Make a JSON payload from it
             json_payload = json.loads(in_obj.json())
 
             # Record it
             self.in_resources.append(
-                dict(guid=guid, model=in_model.__name__, payload=json_payload)
+                dict(guid=guid, model=in_obj.__class__.__name__, payload=json_payload)
             )
 
         return self.in_resources
 
 
 class PackageInstaller:
     statuses = {1: "created", 0: "existing", -1: "error"}
```

### Comparing `bpkio_cli-1.1.0/bpkio_cli/core/resource_recorder.py` & `bpkio_cli-1.2.0/bpkio_cli/core/resource_recorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         if value == "$":
             last_id = self.last_id_by_type(target_type)
             if last_id:
                 return str(last_id)
             else:
                 raise ValueError(
                     "There is no resource in memory that can be found to "
-                    "replace '$' for this context"
+                    "replace '$' for this context. It may have been deleted"
                 )
 
         if value.startswith("@"):
             match = re.search(r"(-?\d+)", value)
             if match:
                 pos = int(match.group(1))
                 id = self.id_by_position_in_last_list_by_type(target_type, pos)
```

### Comparing `bpkio_cli-1.1.0/bpkio_cli/core/resources_context.py` & `bpkio_cli-1.2.0/bpkio_cli/core/resources_context.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/core/response_handler.py` & `bpkio_cli-1.2.0/bpkio_cli/core/response_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,18 +89,19 @@
             data = j.loads(resource.json(exclude_none=False))
             colored_json = JSONFormatter().format(data)
             click.echo(colored_json)
 
             return resource
 
         elif not isinstance(resource, BaseResource):
-            data = j.dumps(resource, indent=2)
-            colored_json = JSONFormatter().format(data)
+            colored_json = JSONFormatter().format(resource)
             click.echo(colored_json)
 
+            return resource
+
         else:
             rows = []
 
             # Identifier
             header = "{} {}".format(
                 click.style(resource.__class__.__name__, fg="white", dim=True),
                 click.style(resource.id, fg="white"),
```

### Comparing `bpkio_cli-1.1.0/bpkio_cli/options/__init__.py` & `bpkio_cli-1.2.0/bpkio_cli/options/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/options/list.py` & `bpkio_cli-1.2.0/bpkio_cli/options/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/options/poll.py` & `bpkio_cli-1.2.0/bpkio_cli/options/poll.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/options/read.py` & `bpkio_cli-1.2.0/bpkio_cli/options/read.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/options/search.py` & `bpkio_cli-1.2.0/bpkio_cli/options/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/options/urls.py` & `bpkio_cli-1.2.0/bpkio_cli/options/urls.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/utils/arrays.py` & `bpkio_cli-1.2.0/bpkio_cli/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/utils/config_provider.py` & `bpkio_cli-1.2.0/bpkio_cli/utils/config_provider.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/utils/datetimes.py` & `bpkio_cli-1.2.0/bpkio_cli/utils/datetimes.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/utils/profile_maker.py` & `bpkio_cli-1.2.0/bpkio_cli/utils/profile_maker.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/utils/url_builders.py` & `bpkio_cli-1.2.0/bpkio_cli/utils/url_builders.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/utils/urls.py` & `bpkio_cli-1.2.0/bpkio_cli/utils/urls.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/writers/breadcrumbs.py` & `bpkio_cli-1.2.0/bpkio_cli/writers/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/writers/colorizer.py` & `bpkio_cli-1.2.0/bpkio_cli/writers/colorizer.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/writers/content_display.py` & `bpkio_cli-1.2.0/bpkio_cli/writers/content_display.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/writers/diff.py` & `bpkio_cli-1.2.0/bpkio_cli/writers/diff.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/writers/hls_formatter.py` & `bpkio_cli-1.2.0/bpkio_cli/writers/hls_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/writers/json_formatter.py` & `bpkio_cli-1.2.0/bpkio_cli/writers/json_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/writers/players.py` & `bpkio_cli-1.2.0/bpkio_cli/writers/players.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/writers/tables.py` & `bpkio_cli-1.2.0/bpkio_cli/writers/tables.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/bpkio_cli/writers/xml_formatter.py` & `bpkio_cli-1.2.0/bpkio_cli/writers/xml_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.1.0/pyproject.toml` & `bpkio_cli-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [tool.poetry]
 name = "bpkio-cli"
-version = "1.1.0"
+version = "1.2.0"
 description = "A command line interface to the broadpeak.io APIs, with additional helpers"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_cli" }]
 
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["*/__init__.py", "*/__version__.py", "*/_version.py"]
 
 [tool.poetry.dependencies]
-# bpkio-python-sdk = { path = "../bpkio-python-sdk", develop = true }
-bpkio-python-sdk = "^1.0.1"
+bpkio-python-sdk = "^1.1.0"
 python = "^3.10"
 click = "^8.1.3"
 colorama = "^0.4.6"
 # inquirerpy = { git = "https://github.com/kazhala/InquirerPy" }
 inquirerpy = "^0.3.4"
 tabulate = "^0.9.0"
 arrow = "^1.2.3"
@@ -31,14 +30,15 @@
 pygments = "^2.15.1"
 
 [tool.poetry.scripts]
 bic = "bpkio_cli.__main__:safe_entry_point"
 bic-debug = "bpkio_cli.__main__:debug_entry_point"
 
 [tool.poetry.group.dev.dependencies]
+bpkio-python-sdk = { path = "../bpkio-python-sdk", develop = true }
 pytest = "^7.2.2"
 black = "^23.1.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
```

### Comparing `bpkio_cli-1.1.0/PKG-INFO` & `bpkio_cli-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bpkio-cli
-Version: 1.1.0
+Version: 1.2.0
 Summary: A command line interface to the broadpeak.io APIs, with additional helpers
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
-Requires-Dist: bpkio-python-sdk (>=1.0.1,<2.0.0)
+Requires-Dist: bpkio-python-sdk (>=1.1.0,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloup (>=2.0.0.post1,<3.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: diskcache (>=5.4.0,<6.0.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
```

