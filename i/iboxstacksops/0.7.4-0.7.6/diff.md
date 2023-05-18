# Comparing `tmp/iboxstacksops-0.7.4.tar.gz` & `tmp/iboxstacksops-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iboxstacksops-0.7.4.tar", last modified: Thu May 11 16:42:50 2023, max compression
+gzip compressed data, was "iboxstacksops-0.7.6.tar", last modified: Thu May 18 16:15:15 2023, max compression
```

## Comparing `iboxstacksops-0.7.4.tar` & `iboxstacksops-0.7.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:42:50.073798 iboxstacksops-0.7.4/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-11 16:42:50.073798 iboxstacksops-0.7.4/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.7.4/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:42:50.061797 iboxstacksops-0.7.4/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:42:50.061797 iboxstacksops-0.7.4/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:42:50.065797 iboxstacksops-0.7.4/build/lib/iboxstacksops.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-11 16:42:49.000000 iboxstacksops-0.7.4/build/lib/iboxstacksops.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-05-11 16:42:49.000000 iboxstacksops-0.7.4/build/lib/iboxstacksops.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-05-11 16:42:49.000000 iboxstacksops-0.7.4/build/lib/iboxstacksops.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-05-11 16:42:49.000000 iboxstacksops-0.7.4/build/lib/iboxstacksops.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-05-11 16:42:49.000000 iboxstacksops-0.7.4/build/lib/iboxstacksops.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:42:50.073798 iboxstacksops-0.7.4/iboxstacksops/
--rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.7.4/iboxstacksops/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.7.4/iboxstacksops/actions.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.7.4/iboxstacksops/aws.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4077 2023-05-11 16:41:05.000000 iboxstacksops-0.7.4/iboxstacksops/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5343 2023-03-30 13:07:04.000000 iboxstacksops-0.7.4/iboxstacksops/changeset.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4186 2023-03-29 07:47:32.000000 iboxstacksops-0.7.4/iboxstacksops/commands.py
--rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.7.4/iboxstacksops/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.7.4/iboxstacksops/dashboard.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.7.4/iboxstacksops/events.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.7.4/iboxstacksops/i_region.py
--rw-r--r--   0 mello     (1000) mello     (1000)     6241 2023-04-11 14:33:36.000000 iboxstacksops-0.7.4/iboxstacksops/i_stack.py
--rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.7.4/iboxstacksops/msg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1299 2021-09-05 11:44:37.000000 iboxstacksops-0.7.4/iboxstacksops/outputs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8666 2023-04-11 14:46:17.000000 iboxstacksops-0.7.4/iboxstacksops/parameters.py
--rw-r--r--   0 mello     (1000) mello     (1000)    17319 2023-05-11 13:23:25.000000 iboxstacksops-0.7.4/iboxstacksops/parser.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.7.4/iboxstacksops/replica.py
--rw-r--r--   0 mello     (1000) mello     (1000)    10010 2023-04-27 12:45:52.000000 iboxstacksops-0.7.4/iboxstacksops/resolve.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.7.4/iboxstacksops/resources.py
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.7.4/iboxstacksops/route53.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.7.4/iboxstacksops/ssm.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.7.4/iboxstacksops/stacks.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1090 2023-03-28 16:37:37.000000 iboxstacksops-0.7.4/iboxstacksops/table.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2836 2023-04-27 16:30:50.000000 iboxstacksops-0.7.4/iboxstacksops/tags.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.7.4/iboxstacksops/template.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.7.4/iboxstacksops/tools.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-11 16:42:50.073798 iboxstacksops-0.7.4/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.7.4/scripts/ibox_stacksops.py
--rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-05-11 16:42:50.077798 iboxstacksops-0.7.4/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-05-11 16:41:46.000000 iboxstacksops-0.7.4/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.073178 iboxstacksops-0.7.6/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-18 16:15:15.073178 iboxstacksops-0.7.6/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.7.6/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.053177 iboxstacksops-0.7.6/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.053177 iboxstacksops-0.7.6/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.061178 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-18 16:15:14.000000 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-05-18 16:15:14.000000 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-05-18 16:15:14.000000 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-05-18 16:15:14.000000 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-05-18 16:15:14.000000 iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.073178 iboxstacksops-0.7.6/iboxstacksops/
+-rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.7.6/iboxstacksops/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.7.6/iboxstacksops/actions.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.7.6/iboxstacksops/aws.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4077 2023-05-11 16:41:05.000000 iboxstacksops-0.7.6/iboxstacksops/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5474 2023-05-18 16:13:00.000000 iboxstacksops-0.7.6/iboxstacksops/changeset.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4186 2023-03-29 07:47:32.000000 iboxstacksops-0.7.6/iboxstacksops/commands.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.7.6/iboxstacksops/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.7.6/iboxstacksops/dashboard.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.7.6/iboxstacksops/events.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.7.6/iboxstacksops/i_region.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     6241 2023-04-11 14:33:36.000000 iboxstacksops-0.7.6/iboxstacksops/i_stack.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.7.6/iboxstacksops/msg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1299 2021-09-05 11:44:37.000000 iboxstacksops-0.7.6/iboxstacksops/outputs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8666 2023-04-11 14:46:17.000000 iboxstacksops-0.7.6/iboxstacksops/parameters.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    17319 2023-05-11 13:23:25.000000 iboxstacksops-0.7.6/iboxstacksops/parser.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.7.6/iboxstacksops/replica.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    10010 2023-04-27 12:45:52.000000 iboxstacksops-0.7.6/iboxstacksops/resolve.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.7.6/iboxstacksops/resources.py
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.7.6/iboxstacksops/route53.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.7.6/iboxstacksops/ssm.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.7.6/iboxstacksops/stacks.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1090 2023-03-28 16:37:37.000000 iboxstacksops-0.7.6/iboxstacksops/table.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2836 2023-04-27 16:30:50.000000 iboxstacksops-0.7.6/iboxstacksops/tags.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.7.6/iboxstacksops/template.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.7.6/iboxstacksops/tools.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-18 16:15:15.073178 iboxstacksops-0.7.6/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.7.6/scripts/ibox_stacksops.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-05-18 16:15:15.073178 iboxstacksops-0.7.6/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-05-18 16:14:44.000000 iboxstacksops-0.7.6/setup.py
```

### Comparing `iboxstacksops-0.7.4/PKG-INFO` & `iboxstacksops-0.7.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.4
+Version: 0.7.6
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.4/build/lib/iboxstacksops.egg-info/PKG-INFO` & `iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.4
+Version: 0.7.6
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.4/build/lib/iboxstacksops.egg-info/SOURCES.txt` & `iboxstacksops-0.7.6/build/lib/iboxstacksops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/actions.py` & `iboxstacksops-0.7.6/iboxstacksops/actions.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/aws.py` & `iboxstacksops-0.7.6/iboxstacksops/aws.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/cfg.py` & `iboxstacksops-0.7.6/iboxstacksops/cfg.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/changeset.py` & `iboxstacksops-0.7.6/iboxstacksops/changeset.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,18 @@
 
 
 # semplify changeset by removing changes where all CausingEntity items will be not replaced
 def _simplify_changeset(changes, not_replaced):
     recurse = False
     for row in list(changes):
         causing_entity = row.get("CausingEntityList", [])
-        if causing_entity and all(
-            n.split(".")[0] in not_replaced for n in causing_entity
+        if (
+            causing_entity
+            and all(n.split(".")[0] in not_replaced for n in causing_entity)
+            and len(row.get("Target", [])) <= len(row.get("CausingEntityList", []))
         ):
             not_replaced.append(row["LogicalResourceId"])
             changes.remove(row)
             recurse = True
     if recurse:
         return _simplify_changeset(changes, not_replaced)
 
@@ -120,18 +122,18 @@
     )
 
     return response
 
 
 # change list in a string new line separated element
 def list_to_string_list(mylist):
-    joined_string = "\n".join(mylist)
-    mystring = joined_string if len(mylist) < 2 else f"({joined_string})"
-
-    return mystring
+    return ",".join(mylist)
+    # joined_string = "\n".join(mylist)
+    # mystring = joined_string if len(mylist) < 2 else f"({joined_string})"
+    # return mystring
 
 
 def process(istack, us_args):
     # -create changeset
     changeset_id = _do_changeset(istack, us_args.copy())
     print("\n")
     istack.mylog("ChangeSetId: %s" % changeset_id)
```

### Comparing `iboxstacksops-0.7.4/iboxstacksops/commands.py` & `iboxstacksops-0.7.6/iboxstacksops/commands.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/common.py` & `iboxstacksops-0.7.6/iboxstacksops/common.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/dashboard.py` & `iboxstacksops-0.7.6/iboxstacksops/dashboard.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/events.py` & `iboxstacksops-0.7.6/iboxstacksops/events.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/i_region.py` & `iboxstacksops-0.7.6/iboxstacksops/i_region.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/i_stack.py` & `iboxstacksops-0.7.6/iboxstacksops/i_stack.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/msg.py` & `iboxstacksops-0.7.6/iboxstacksops/msg.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/outputs.py` & `iboxstacksops-0.7.6/iboxstacksops/outputs.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/parameters.py` & `iboxstacksops-0.7.6/iboxstacksops/parameters.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/parser.py` & `iboxstacksops-0.7.6/iboxstacksops/parser.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/replica.py` & `iboxstacksops-0.7.6/iboxstacksops/replica.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/resolve.py` & `iboxstacksops-0.7.6/iboxstacksops/resolve.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/resources.py` & `iboxstacksops-0.7.6/iboxstacksops/resources.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/route53.py` & `iboxstacksops-0.7.6/iboxstacksops/route53.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/ssm.py` & `iboxstacksops-0.7.6/iboxstacksops/ssm.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/stacks.py` & `iboxstacksops-0.7.6/iboxstacksops/stacks.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/table.py` & `iboxstacksops-0.7.6/iboxstacksops/table.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/tags.py` & `iboxstacksops-0.7.6/iboxstacksops/tags.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/template.py` & `iboxstacksops-0.7.6/iboxstacksops/template.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/iboxstacksops/tools.py` & `iboxstacksops-0.7.6/iboxstacksops/tools.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.4/setup.py` & `iboxstacksops-0.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iboxstacksops",
-    version="0.7.4",
+    version="0.7.6",
     author="Mello",
     author_email="mello+python@ankot.org",
     description="AWS Infrastructure in a Box - Stacks management program",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mello7tre/AwsIBoxStackOps",
     packages=["iboxstacksops",],
```

