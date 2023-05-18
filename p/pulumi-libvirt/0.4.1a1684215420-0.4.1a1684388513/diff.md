# Comparing `tmp/pulumi_libvirt-0.4.1a1684215420.tar.gz` & `tmp/pulumi_libvirt-0.4.1a1684388513.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_libvirt-0.4.1a1684215420.tar", last modified: Tue May 16 05:44:45 2023, max compression
+gzip compressed data, was "pulumi_libvirt-0.4.1a1684388513.tar", last modified: Thu May 18 05:50:08 2023, max compression
```

## Comparing `pulumi_libvirt-0.4.1a1684215420.tar` & `pulumi_libvirt-0.4.1a1684388513.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:44:45.475769 pulumi_libvirt-0.4.1a1684215420/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-16 05:44:45.475769 pulumi_libvirt-0.4.1a1684215420/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:44:45.475769 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45336 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/cloud_init_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:44:45.475769 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    72754 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/get_network_dns_host_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/get_network_dns_srv_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/get_network_dnsmasq_options_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/ignition.py
--rw-r--r--   0 runner    (1001) docker     (123)    34091 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    38775 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:44:45.475769 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 05:44:45.475769 pulumi_libvirt-0.4.1a1684215420/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 05:44:45.000000 pulumi_libvirt-0.4.1a1684215420/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:50:08.858676 pulumi_libvirt-0.4.1a1684388513/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-18 05:50:08.858676 pulumi_libvirt-0.4.1a1684388513/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:50:08.854676 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45336 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/cloud_init_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:50:08.858676 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72754 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/get_network_dns_host_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/get_network_dns_srv_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/get_network_dnsmasq_options_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/ignition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34091 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38775 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:50:08.858676 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 05:50:08.858676 pulumi_libvirt-0.4.1a1684388513/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-18 05:50:08.000000 pulumi_libvirt-0.4.1a1684388513/setup.py
```

### Comparing `pulumi_libvirt-0.4.1a1684215420/PKG-INFO` & `pulumi_libvirt-0.4.1a1684388513/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.4.1a1684215420
+Version: 0.4.1a1684388513
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi libvirt
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_libvirt-0.4.1a1684215420/README.md` & `pulumi_libvirt-0.4.1a1684388513/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/__init__.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/_inputs.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/_utilities.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/cloud_init_disk.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/cloud_init_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/config/vars.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/domain.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/get_network_dns_host_template.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/get_network_dns_host_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/get_network_dns_srv_template.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/get_network_dns_srv_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/get_network_dnsmasq_options_template.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/get_network_dnsmasq_options_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/ignition.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/ignition.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/network.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/outputs.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/pool.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/provider.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt/volume.py` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt.egg-info/PKG-INFO` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-libvirt
-Version: 0.4.1a1684215420
+Version: 0.4.1a1684388513
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi libvirt
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_libvirt-0.4.1a1684215420/pulumi_libvirt.egg-info/SOURCES.txt` & `pulumi_libvirt-0.4.1a1684388513/pulumi_libvirt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1684215420/setup.py` & `pulumi_libvirt-0.4.1a1684388513/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.1a1684215420"
-PLUGIN_VERSION = "0.4.1-alpha.1684215420+f5027d40"
+VERSION = "0.4.1a1684388513"
+PLUGIN_VERSION = "0.4.1-alpha.1684388513+cafc7255"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'libvirt', PLUGIN_VERSION])
         except OSError as error:
```

