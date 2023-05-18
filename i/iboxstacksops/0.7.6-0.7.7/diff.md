# Comparing `tmp/iboxstacksops-0.7.6.tar.gz` & `tmp/iboxstacksops-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iboxstacksops-0.7.6.tar", last modified: Thu May 18 16:15:15 2023, max compression
+gzip compressed data, was "iboxstacksops-0.7.7.tar", last modified: Thu May 18 19:43:16 2023, max compression
```

## Comparing `iboxstacksops-0.7.6.tar` & `iboxstacksops-0.7.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.073178 iboxstacksops-0.7.6/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-18 16:15:15.073178 iboxstacksops-0.7.6/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.7.6/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.053177 iboxstacksops-0.7.6/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.053177 iboxstacksops-0.7.6/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.061178 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-18 16:15:14.000000 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-05-18 16:15:14.000000 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-05-18 16:15:14.000000 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-05-18 16:15:14.000000 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-05-18 16:15:14.000000 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.073178 iboxstacksops-0.7.6/iboxstacksops/
--rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.7.6/iboxstacksops/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.7.6/iboxstacksops/actions.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.7.6/iboxstacksops/aws.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4077 2023-05-11 16:41:05.000000 iboxstacksops-0.7.6/iboxstacksops/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5474 2023-05-18 16:13:00.000000 iboxstacksops-0.7.6/iboxstacksops/changeset.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4186 2023-03-29 07:47:32.000000 iboxstacksops-0.7.6/iboxstacksops/commands.py
--rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.7.6/iboxstacksops/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.7.6/iboxstacksops/dashboard.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.7.6/iboxstacksops/events.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.7.6/iboxstacksops/i_region.py
--rw-r--r--   0 mello     (1000) mello     (1000)     6241 2023-04-11 14:33:36.000000 iboxstacksops-0.7.6/iboxstacksops/i_stack.py
--rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.7.6/iboxstacksops/msg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1299 2021-09-05 11:44:37.000000 iboxstacksops-0.7.6/iboxstacksops/outputs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8666 2023-04-11 14:46:17.000000 iboxstacksops-0.7.6/iboxstacksops/parameters.py
--rw-r--r--   0 mello     (1000) mello     (1000)    17319 2023-05-11 13:23:25.000000 iboxstacksops-0.7.6/iboxstacksops/parser.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.7.6/iboxstacksops/replica.py
--rw-r--r--   0 mello     (1000) mello     (1000)    10010 2023-04-27 12:45:52.000000 iboxstacksops-0.7.6/iboxstacksops/resolve.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.7.6/iboxstacksops/resources.py
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.7.6/iboxstacksops/route53.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.7.6/iboxstacksops/ssm.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.7.6/iboxstacksops/stacks.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1090 2023-03-28 16:37:37.000000 iboxstacksops-0.7.6/iboxstacksops/table.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2836 2023-04-27 16:30:50.000000 iboxstacksops-0.7.6/iboxstacksops/tags.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.7.6/iboxstacksops/template.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.7.6/iboxstacksops/tools.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.073178 iboxstacksops-0.7.6/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.7.6/scripts/ibox_stacksops.py
--rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-05-18 16:15:15.073178 iboxstacksops-0.7.6/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-05-18 16:14:44.000000 iboxstacksops-0.7.6/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.663079 iboxstacksops-0.7.7/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-18 19:43:16.663079 iboxstacksops-0.7.7/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.7.7/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.651079 iboxstacksops-0.7.7/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.651079 iboxstacksops-0.7.7/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.655079 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-18 19:43:16.000000 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-05-18 19:43:16.000000 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-05-18 19:43:16.000000 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-05-18 19:43:16.000000 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-05-18 19:43:16.000000 iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.663079 iboxstacksops-0.7.7/iboxstacksops/
+-rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.7.7/iboxstacksops/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.7.7/iboxstacksops/actions.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.7.7/iboxstacksops/aws.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4077 2023-05-11 16:41:05.000000 iboxstacksops-0.7.7/iboxstacksops/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5474 2023-05-18 16:13:00.000000 iboxstacksops-0.7.7/iboxstacksops/changeset.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4234 2023-05-18 19:15:17.000000 iboxstacksops-0.7.7/iboxstacksops/commands.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.7.7/iboxstacksops/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.7.7/iboxstacksops/dashboard.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.7.7/iboxstacksops/events.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.7.7/iboxstacksops/i_region.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     6428 2023-05-18 19:31:13.000000 iboxstacksops-0.7.7/iboxstacksops/i_stack.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.7.7/iboxstacksops/msg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1349 2023-05-18 19:03:13.000000 iboxstacksops-0.7.7/iboxstacksops/outputs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8715 2023-05-18 19:03:44.000000 iboxstacksops-0.7.7/iboxstacksops/parameters.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    17319 2023-05-11 13:23:25.000000 iboxstacksops-0.7.7/iboxstacksops/parser.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.7.7/iboxstacksops/replica.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    10010 2023-04-27 12:45:52.000000 iboxstacksops-0.7.7/iboxstacksops/resolve.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.7.7/iboxstacksops/resources.py
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.7.7/iboxstacksops/route53.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.7.7/iboxstacksops/ssm.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.7.7/iboxstacksops/stacks.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1090 2023-03-28 16:37:37.000000 iboxstacksops-0.7.7/iboxstacksops/table.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2836 2023-04-27 16:30:50.000000 iboxstacksops-0.7.7/iboxstacksops/tags.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.7.7/iboxstacksops/template.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.7.7/iboxstacksops/tools.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 19:43:16.663079 iboxstacksops-0.7.7/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.7.7/scripts/ibox_stacksops.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-05-18 19:43:16.663079 iboxstacksops-0.7.7/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-05-18 19:42:22.000000 iboxstacksops-0.7.7/setup.py
```

### Comparing `iboxstacksops-0.7.6/PKG-INFO` & `iboxstacksops-0.7.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.6
+Version: 0.7.7
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/PKG-INFO` & `iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.6
+Version: 0.7.7
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/SOURCES.txt` & `iboxstacksops-0.7.7/build/lib/iboxstacksops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/actions.py` & `iboxstacksops-0.7.7/iboxstacksops/actions.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/aws.py` & `iboxstacksops-0.7.7/iboxstacksops/aws.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/cfg.py` & `iboxstacksops-0.7.7/iboxstacksops/cfg.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/changeset.py` & `iboxstacksops-0.7.7/iboxstacksops/changeset.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/commands.py` & `iboxstacksops-0.7.7/iboxstacksops/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,20 +72,21 @@
 
 def parameters():
     w_stacks = stacks.get()
     cfg.exports = get_exports()
     result = concurrent_exec("parameters", w_stacks, i_stack)
 
 
-def info():
+def info(mylog=True):
     if not cfg.compact:
         cfg.OUT_WIDTH = 80
     w_stacks = stacks.get()
-    result = concurrent_exec("info", w_stacks, i_stack)
+    result = concurrent_exec("info", w_stacks, i_stack, **{"mylog": mylog})
 
+    return result
 
 def show_resources():
     w_stacks = stacks.get()
     result = concurrent_exec("show_resources", w_stacks, i_stack)
 
 
 def log():
```

### Comparing `iboxstacksops-0.7.6/iboxstacksops/common.py` & `iboxstacksops-0.7.7/iboxstacksops/common.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/dashboard.py` & `iboxstacksops-0.7.7/iboxstacksops/dashboard.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/events.py` & `iboxstacksops-0.7.7/iboxstacksops/events.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/i_region.py` & `iboxstacksops-0.7.7/iboxstacksops/i_region.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/i_stack.py` & `iboxstacksops-0.7.7/iboxstacksops/i_stack.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,19 +95,24 @@
         if check:
             parameters.add_stack_params_as_args(self, parser)
             return self.stack_parsed_args, self.parameters
         else:
             logger.info(f"{self.name} Parameters:")
             parser.print_help()
 
-    def info(self):
+    def info(self, mylog=True):
         self.stack = self.cloudformation.Stack(self.name)
         self.template = template.get_template(self)
-        outputs.show(self, "before")
-        parameters.show_override(self)
+        outputs_out = outputs.show(self, "before", mylog=mylog)
+        parameters_out = parameters.show_override(self, mylog=mylog)
+
+        return {
+            "OUTPUTS": outputs_out,
+            "PARAMETERS NOT DEFAULT": parameters_out,
+        }
 
     def show_resources(self):
         self.stack = self.cloudformation.Stack(self.name)
         result = actions.show_resources(self)
 
     def log(self):
         self.stack = self.cloudformation.Stack(self.name)
```

### Comparing `iboxstacksops-0.7.6/iboxstacksops/msg.py` & `iboxstacksops-0.7.7/iboxstacksops/msg.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/outputs.py` & `iboxstacksops-0.7.7/iboxstacksops/outputs.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,20 +16,23 @@
 
     istack.changed["outputs"] = changed
     istack.cfg.OUT_WIDTH = 80
     show(istack, "changed")
 
 
 # show stack current outputs as dict
-def show(istack, when):
+def show(istack, when, mylog=True):
     outputs = getattr(istack, when)["outputs"]
 
     out = pformat(outputs, width=istack.cfg.OUT_WIDTH)
 
-    istack.mylog(f"{when.upper()} - STACK OUTPUTS\n{out}\n")
+    if mylog:
+        istack.mylog(f"{when.upper()} - STACK OUTPUTS\n{out}\n")
+
+    return outputs
 
 
 def get(stack):
     outputs = {}
 
     try:
         stack["StackName"]
```

### Comparing `iboxstacksops-0.7.6/iboxstacksops/parameters.py` & `iboxstacksops-0.7.7/iboxstacksops/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,30 +154,33 @@
     istack.stack_parsed_args = args
 
     for n, v in vars(args).items():
         if not hasattr(istack.cfg, n):
             setattr(istack.cfg, n, v)
 
 
-def show_override(istack):
+def show_override(istack, mylog=True):
     params = {}
     for name, value in istack.c_parameters.items():
         if (
             not name.startswith("Env")
             and any(name not in n for n in ["UpdateMode"])
             and any(
                 name == t_name and (value != t_value.get("Default"))
                 for t_name, t_value in istack.parameters.items()
             )
         ):
             params[name] = value
 
     out = pformat(params, width=istack.cfg.OUT_WIDTH)
 
-    istack.mylog(f"CURRENT NOT DEFAULT - STACK PARAMETERS\n{out}\n")
+    if mylog:
+        istack.mylog(f"CURRENT NOT DEFAULT - STACK PARAMETERS\n{out}\n")
+
+    return params
 
 
 def process(istack, show=True):
     logger.info("Processing Parameters")
 
     # get stack parameter parser
     parser = get_stack_parameter_parser(istack)
```

### Comparing `iboxstacksops-0.7.6/iboxstacksops/parser.py` & `iboxstacksops-0.7.7/iboxstacksops/parser.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/replica.py` & `iboxstacksops-0.7.7/iboxstacksops/replica.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/resolve.py` & `iboxstacksops-0.7.7/iboxstacksops/resolve.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/resources.py` & `iboxstacksops-0.7.7/iboxstacksops/resources.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/route53.py` & `iboxstacksops-0.7.7/iboxstacksops/route53.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/ssm.py` & `iboxstacksops-0.7.7/iboxstacksops/ssm.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/stacks.py` & `iboxstacksops-0.7.7/iboxstacksops/stacks.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/table.py` & `iboxstacksops-0.7.7/iboxstacksops/table.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/tags.py` & `iboxstacksops-0.7.7/iboxstacksops/tags.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/template.py` & `iboxstacksops-0.7.7/iboxstacksops/template.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/iboxstacksops/tools.py` & `iboxstacksops-0.7.7/iboxstacksops/tools.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.6/setup.py` & `iboxstacksops-0.7.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iboxstacksops",
-    version="0.7.6",
+    version="0.7.7",
     author="Mello",
     author_email="mello+python@ankot.org",
     description="AWS Infrastructure in a Box - Stacks management program",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mello7tre/AwsIBoxStackOps",
     packages=["iboxstacksops",],
```

