# Comparing `tmp/pulumi_containerregistry-0.0.6.tar.gz` & `tmp/pulumi_containerregistry-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_containerregistry-0.0.6.tar", last modified: Wed May 17 22:32:29 2023, max compression
+gzip compressed data, was "pulumi_containerregistry-0.0.7.tar", last modified: Wed May 17 23:08:41 2023, max compression
```

## Comparing `pulumi_containerregistry-0.0.6.tar` & `pulumi_containerregistry-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:32:29.019995 pulumi_containerregistry-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 22:32:29.019995 pulumi_containerregistry-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:32:29.019995 pulumi_containerregistry-0.0.6/pulumi_containerregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:32:29.019995 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 22:32:29.000000 pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:32:29.019995 pulumi_containerregistry-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-17 22:32:28.000000 pulumi_containerregistry-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:08:41.161074 pulumi_containerregistry-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 23:08:41.161074 pulumi_containerregistry-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-05-17 23:08:40.000000 pulumi_containerregistry-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:08:41.161074 pulumi_containerregistry-0.0.7/pulumi_containerregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 23:08:40.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-05-17 23:08:40.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-17 23:08:40.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 23:08:40.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 23:08:40.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-17 23:08:40.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:08:41.161074 pulumi_containerregistry-0.0.7/pulumi_containerregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-05-17 23:08:41.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-17 23:08:41.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 23:08:41.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 23:08:41.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 23:08:41.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 23:08:41.000000 pulumi_containerregistry-0.0.7/pulumi_containerregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 23:08:41.161074 pulumi_containerregistry-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-17 23:08:40.000000 pulumi_containerregistry-0.0.7/setup.py
```

### Comparing `pulumi_containerregistry-0.0.6/PKG-INFO` & `pulumi_containerregistry-0.0.7/pulumi_containerregistry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_containerregistry
-Version: 0.0.6
+Name: pulumi-containerregistry
+Version: 0.0.7
 Summary: A Pulumi package for creating and managing containerregistry cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/rhysmdnz/pulumi-containerregistry
 Keywords: pulumi containerregistry category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_containerregistry-0.0.6/README.md` & `pulumi_containerregistry-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.6/pulumi_containerregistry/__init__.py` & `pulumi_containerregistry-0.0.7/pulumi_containerregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.6/pulumi_containerregistry/_utilities.py` & `pulumi_containerregistry-0.0.7/pulumi_containerregistry/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.6/pulumi_containerregistry/provider.py` & `pulumi_containerregistry-0.0.7/pulumi_containerregistry/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.6/pulumi_containerregistry/resource.py` & `pulumi_containerregistry-0.0.7/pulumi_containerregistry/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,38 +10,27 @@
 from . import _utilities
 
 __all__ = ['ResourceArgs', 'Resource']
 
 @pulumi.input_type
 class ResourceArgs:
     def __init__(__self__, *,
-                 image_tarball_hash: pulumi.Input[str],
                  image_tarball: pulumi.Input[Union[pulumi.Asset, pulumi.Archive]],
-                 remote_tag: pulumi.Input[str]):
+                 remote_tag: pulumi.Input[str],
+                 image_tarball_hash: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Resource resource.
-        :param pulumi.Input[str] image_tarball_hash: Hash of the image tarball.
         :param pulumi.Input[Union[pulumi.Asset, pulumi.Archive]] image_tarball: Image tarball thing.
         :param pulumi.Input[str] remote_tag: The tag to save the image to.
+        :param pulumi.Input[str] image_tarball_hash: Hash of the image tarball.
         """
-        pulumi.set(__self__, "image_tarball_hash", image_tarball_hash)
         pulumi.set(__self__, "image_tarball", image_tarball)
         pulumi.set(__self__, "remote_tag", remote_tag)
-
-    @property
-    @pulumi.getter(name="imageTarballHash")
-    def image_tarball_hash(self) -> pulumi.Input[str]:
-        """
-        Hash of the image tarball.
-        """
-        return pulumi.get(self, "image_tarball_hash")
-
-    @image_tarball_hash.setter
-    def image_tarball_hash(self, value: pulumi.Input[str]):
-        pulumi.set(self, "image_tarball_hash", value)
+        if image_tarball_hash is not None:
+            pulumi.set(__self__, "image_tarball_hash", image_tarball_hash)
 
     @property
     @pulumi.getter
     def image_tarball(self) -> pulumi.Input[Union[pulumi.Asset, pulumi.Archive]]:
         """
         Image tarball thing.
         """
@@ -59,14 +48,26 @@
         """
         return pulumi.get(self, "remote_tag")
 
     @remote_tag.setter
     def remote_tag(self, value: pulumi.Input[str]):
         pulumi.set(self, "remote_tag", value)
 
+    @property
+    @pulumi.getter(name="imageTarballHash")
+    def image_tarball_hash(self) -> Optional[pulumi.Input[str]]:
+        """
+        Hash of the image tarball.
+        """
+        return pulumi.get(self, "image_tarball_hash")
+
+    @image_tarball_hash.setter
+    def image_tarball_hash(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "image_tarball_hash", value)
+
 
 @pulumi.input_type
 class _ResourceState:
     def __init__(__self__, *,
                  image_tarball_hash: Optional[pulumi.Input[str]] = None,
                  image_tarball: Optional[pulumi.Input[Union[pulumi.Asset, pulumi.Archive]]] = None,
                  remote_tag: Optional[pulumi.Input[str]] = None):
@@ -168,16 +169,14 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ResourceArgs.__new__(ResourceArgs)
 
-            if image_tarball_hash is None and not opts.urn:
-                raise TypeError("Missing required property 'image_tarball_hash'")
             __props__.__dict__["image_tarball_hash"] = image_tarball_hash
             if image_tarball is None and not opts.urn:
                 raise TypeError("Missing required property 'image_tarball'")
             __props__.__dict__["image_tarball"] = image_tarball
             if remote_tag is None and not opts.urn:
                 raise TypeError("Missing required property 'remote_tag'")
             __props__.__dict__["remote_tag"] = remote_tag
@@ -212,15 +211,15 @@
         __props__.__dict__["image_tarball_hash"] = image_tarball_hash
         __props__.__dict__["image_tarball"] = image_tarball
         __props__.__dict__["remote_tag"] = remote_tag
         return Resource(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="imageTarballHash")
-    def image_tarball_hash(self) -> pulumi.Output[str]:
+    def image_tarball_hash(self) -> pulumi.Output[Optional[str]]:
         """
         Hash of the image tarball.
         """
         return pulumi.get(self, "image_tarball_hash")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/PKG-INFO` & `pulumi_containerregistry-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-containerregistry
-Version: 0.0.6
+Name: pulumi_containerregistry
+Version: 0.0.7
 Summary: A Pulumi package for creating and managing containerregistry cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/rhysmdnz/pulumi-containerregistry
 Keywords: pulumi containerregistry category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_containerregistry-0.0.6/pulumi_containerregistry.egg-info/SOURCES.txt` & `pulumi_containerregistry-0.0.7/pulumi_containerregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_containerregistry-0.0.6/setup.py` & `pulumi_containerregistry-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.6"
-PLUGIN_VERSION = "0.0.6"
+VERSION = "0.0.7"
+PLUGIN_VERSION = "0.0.7"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'containerregistry', PLUGIN_VERSION, '--server', 'github://api.github.com/rhysmdnz/pulumi-containerregistry'])
         except OSError as error:
```

