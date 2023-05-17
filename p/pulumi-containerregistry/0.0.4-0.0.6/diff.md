# Comparing `tmp/pulumi_containerregistry-0.0.4.tar.gz` & `tmp/pulumi_containerregistry-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_containerregistry-0.0.4.tar", last modified: Wed May 17 13:16:05 2023, max compression
+gzip compressed data, was "pulumi_containerregistry-0.0.6.tar", last modified: Wed May 17 22:32:29 2023, max compression
```

## Comparing `pulumi_containerregistry-0.0.4.tar` & `pulumi_containerregistry-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:16:05.206116 pulumi_containerregistry-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 13:16:05.206116 pulumi_containerregistry-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:16:05.202115 pulumi_containerregistry-0.0.4/pulumi_containerregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:16:05.206116 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 13:16:05.000000 pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:16:05.206116 pulumi_containerregistry-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-17 13:16:04.000000 pulumi_containerregistry-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:32:29.019995 pulumi_containerregistry-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 22:32:29.019995 pulumi_containerregistry-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:32:29.019995 pulumi_containerregistry-0.0.6/pulumi_containerregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:32:29.019995 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:32:29.019995 pulumi_containerregistry-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/setup.py
```

### Comparing `pulumi_containerregistry-0.0.4/PKG-INFO` & `pulumi_containerregistry-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_containerregistry
-Version: 0.0.4
+Version: 0.0.6
 Summary: A Pulumi package for creating and managing containerregistry cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/rhysmdnz/pulumi-containerregistry
 Keywords: pulumi containerregistry category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_containerregistry-0.0.4/README.md` & `pulumi_containerregistry-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.4/pulumi_containerregistry/__init__.py` & `pulumi_containerregistry-0.0.6/pulumi_containerregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.4/pulumi_containerregistry/_utilities.py` & `pulumi_containerregistry-0.0.6/pulumi_containerregistry/_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,8 +243,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return "https://github.com/rhysmdnz/pulumi-containerregistry/releases/"
+	return "github://api.github.com/rhysmdnz/pulumi-containerregistry"
```

### Comparing `pulumi_containerregistry-0.0.4/pulumi_containerregistry/provider.py` & `pulumi_containerregistry-0.0.6/pulumi_containerregistry/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.4/pulumi_containerregistry/resource.py` & `pulumi_containerregistry-0.0.6/pulumi_containerregistry/resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/PKG-INFO` & `pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-containerregistry
-Version: 0.0.4
+Version: 0.0.6
 Summary: A Pulumi package for creating and managing containerregistry cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/rhysmdnz/pulumi-containerregistry
 Keywords: pulumi containerregistry category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_containerregistry-0.0.4/pulumi_containerregistry.egg-info/SOURCES.txt` & `pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.4/setup.py` & `pulumi_containerregistry-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.4"
-PLUGIN_VERSION = "0.0.4"
+VERSION = "0.0.6"
+PLUGIN_VERSION = "0.0.6"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'containerregistry', PLUGIN_VERSION, '--server', 'https://github.com/rhysmdnz/pulumi-containerregistry/releases/'])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'containerregistry', PLUGIN_VERSION, '--server', 'github://api.github.com/rhysmdnz/pulumi-containerregistry'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the containerregistry resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
```

