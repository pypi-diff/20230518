# Comparing `tmp/platinumtools-0.4.tar.gz` & `tmp/platinumtools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platinumtools-0.4.tar", last modified: Thu May 18 14:57:29 2023, max compression
+gzip compressed data, was "platinumtools-0.4.1.tar", last modified: Thu May 18 15:14:19 2023, max compression
```

## Comparing `platinumtools-0.4.tar` & `platinumtools-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 14:57:29.265370 platinumtools-0.4/
--rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.4/LICENSE
--rw-rw-rw-   0        0        0      861 2023-05-18 14:57:29.264373 platinumtools-0.4/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 platinumtools-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 14:57:29.182423 platinumtools-0.4/platinumtools/
--rw-rw-rw-   0        0        0      423 2023-05-16 18:33:49.000000 platinumtools-0.4/platinumtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:57:29.241370 platinumtools-0.4/platinumtools/aws_classes/
--rw-rw-rw-   0        0        0     1246 2023-05-16 15:56:00.000000 platinumtools-0.4/platinumtools/aws_classes/CommonProcesor.py
--rw-rw-rw-   0        0        0     2408 2023-05-16 18:16:53.000000 platinumtools-0.4/platinumtools/aws_classes/JobListener.py
--rw-rw-rw-   0        0        0      190 2023-05-16 18:42:08.000000 platinumtools-0.4/platinumtools/aws_classes/__init__.py
--rw-rw-rw-   0        0        0     2189 2023-04-28 16:22:33.000000 platinumtools-0.4/platinumtools/aws_classes/class_adapters.py
--rw-rw-rw-   0        0        0    28153 2023-05-18 14:55:15.000000 platinumtools-0.4/platinumtools/aws_classes/class_enhancement.py
--rw-rw-rw-   0        0        0     2296 2023-02-16 19:18:53.000000 platinumtools-0.4/platinumtools/aws_classes/class_guardian.py
--rw-rw-rw-   0        0        0    16271 2023-05-17 20:00:11.000000 platinumtools-0.4/platinumtools/aws_classes/class_helpers.py
--rw-rw-rw-   0        0        0     1789 2023-02-21 20:05:33.000000 platinumtools-0.4/platinumtools/aws_classes/class_scheduling.py
--rw-rw-rw-   0        0        0     7191 2023-05-17 16:26:56.000000 platinumtools-0.4/platinumtools/aws_classes/config_mapper.py
--rw-rw-rw-   0        0        0    19732 2023-05-17 16:45:45.000000 platinumtools-0.4/platinumtools/aws_classes/config_mapper_df.py
--rw-rw-rw-   0        0        0    20802 2023-05-17 16:22:55.000000 platinumtools-0.4/platinumtools/dda_constants.py
--rw-rw-rw-   0        0        0     8070 2023-05-17 15:42:43.000000 platinumtools-0.4/platinumtools/dda_models.py
--rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.4/platinumtools/etl_functions.py
--rw-rw-rw-   0        0        0      102 2023-02-15 19:22:28.000000 platinumtools-0.4/platinumtools/help.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:57:29.215819 platinumtools-0.4/platinumtools.egg-info/
--rw-rw-rw-   0        0        0      861 2023-05-18 14:57:28.000000 platinumtools-0.4/platinumtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1081 2023-05-18 14:57:28.000000 platinumtools-0.4/platinumtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 14:57:28.000000 platinumtools-0.4/platinumtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-18 14:57:28.000000 platinumtools-0.4/platinumtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 14:57:29.265370 platinumtools-0.4/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-05-18 14:53:52.000000 platinumtools-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:57:29.263370 platinumtools-0.4/test_scenarios/
--rw-rw-rw-   0        0        0     4592 2023-05-17 18:21:56.000000 platinumtools-0.4/test_scenarios/JobListener.py
--rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 platinumtools-0.4/test_scenarios/__init__.py
--rw-rw-rw-   0        0        0     9421 2023-03-02 14:45:40.000000 platinumtools-0.4/test_scenarios/test_adapters.py
--rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 platinumtools-0.4/test_scenarios/test_code.py
--rw-rw-rw-   0        0        0     4203 2023-05-17 19:56:18.000000 platinumtools-0.4/test_scenarios/test_common_processing.py
--rw-rw-rw-   0        0        0    26979 2023-05-17 15:29:56.000000 platinumtools-0.4/test_scenarios/test_enhancement.py
--rw-rw-rw-   0        0        0    20476 2023-05-17 15:34:29.000000 platinumtools-0.4/test_scenarios/test_event_normalization.py
--rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 platinumtools-0.4/test_scenarios/test_guardian.py
--rw-rw-rw-   0        0        0     4605 2023-05-17 15:23:32.000000 platinumtools-0.4/test_scenarios/test_helpers.py
--rw-rw-rw-   0        0        0     5427 2023-05-17 15:23:32.000000 platinumtools-0.4/test_scenarios/test_scheduling.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:14:19.264866 platinumtools-0.4.1/
+-rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0      863 2023-05-18 15:14:19.263756 platinumtools-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 platinumtools-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 15:14:19.110272 platinumtools-0.4.1/platinumtools/
+-rw-rw-rw-   0        0        0      423 2023-05-16 18:33:49.000000 platinumtools-0.4.1/platinumtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:14:19.188863 platinumtools-0.4.1/platinumtools/aws_classes/
+-rw-rw-rw-   0        0        0     1246 2023-05-16 15:56:00.000000 platinumtools-0.4.1/platinumtools/aws_classes/CommonProcesor.py
+-rw-rw-rw-   0        0        0     2408 2023-05-16 18:16:53.000000 platinumtools-0.4.1/platinumtools/aws_classes/JobListener.py
+-rw-rw-rw-   0        0        0      190 2023-05-16 18:42:08.000000 platinumtools-0.4.1/platinumtools/aws_classes/__init__.py
+-rw-rw-rw-   0        0        0     2189 2023-04-28 16:22:33.000000 platinumtools-0.4.1/platinumtools/aws_classes/class_adapters.py
+-rw-rw-rw-   0        0        0    28146 2023-05-18 15:13:07.000000 platinumtools-0.4.1/platinumtools/aws_classes/class_enhancement.py
+-rw-rw-rw-   0        0        0     2296 2023-02-16 19:18:53.000000 platinumtools-0.4.1/platinumtools/aws_classes/class_guardian.py
+-rw-rw-rw-   0        0        0    16271 2023-05-17 20:00:11.000000 platinumtools-0.4.1/platinumtools/aws_classes/class_helpers.py
+-rw-rw-rw-   0        0        0     1789 2023-02-21 20:05:33.000000 platinumtools-0.4.1/platinumtools/aws_classes/class_scheduling.py
+-rw-rw-rw-   0        0        0     7191 2023-05-17 16:26:56.000000 platinumtools-0.4.1/platinumtools/aws_classes/config_mapper.py
+-rw-rw-rw-   0        0        0    19732 2023-05-17 16:45:45.000000 platinumtools-0.4.1/platinumtools/aws_classes/config_mapper_df.py
+-rw-rw-rw-   0        0        0    20802 2023-05-17 16:22:55.000000 platinumtools-0.4.1/platinumtools/dda_constants.py
+-rw-rw-rw-   0        0        0     8070 2023-05-17 15:42:43.000000 platinumtools-0.4.1/platinumtools/dda_models.py
+-rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.4.1/platinumtools/etl_functions.py
+-rw-rw-rw-   0        0        0      102 2023-02-15 19:22:28.000000 platinumtools-0.4.1/platinumtools/help.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:14:19.142900 platinumtools-0.4.1/platinumtools.egg-info/
+-rw-rw-rw-   0        0        0      863 2023-05-18 15:14:17.000000 platinumtools-0.4.1/platinumtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1081 2023-05-18 15:14:18.000000 platinumtools-0.4.1/platinumtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 15:14:17.000000 platinumtools-0.4.1/platinumtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-18 15:14:18.000000 platinumtools-0.4.1/platinumtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 15:14:19.265378 platinumtools-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-05-18 15:14:09.000000 platinumtools-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:14:19.261189 platinumtools-0.4.1/test_scenarios/
+-rw-rw-rw-   0        0        0     4592 2023-05-17 18:21:56.000000 platinumtools-0.4.1/test_scenarios/JobListener.py
+-rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 platinumtools-0.4.1/test_scenarios/__init__.py
+-rw-rw-rw-   0        0        0     9421 2023-03-02 14:45:40.000000 platinumtools-0.4.1/test_scenarios/test_adapters.py
+-rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 platinumtools-0.4.1/test_scenarios/test_code.py
+-rw-rw-rw-   0        0        0     4203 2023-05-17 19:56:18.000000 platinumtools-0.4.1/test_scenarios/test_common_processing.py
+-rw-rw-rw-   0        0        0    26979 2023-05-17 15:29:56.000000 platinumtools-0.4.1/test_scenarios/test_enhancement.py
+-rw-rw-rw-   0        0        0    20476 2023-05-17 15:34:29.000000 platinumtools-0.4.1/test_scenarios/test_event_normalization.py
+-rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 platinumtools-0.4.1/test_scenarios/test_guardian.py
+-rw-rw-rw-   0        0        0     4605 2023-05-17 15:23:32.000000 platinumtools-0.4.1/test_scenarios/test_helpers.py
+-rw-rw-rw-   0        0        0     5427 2023-05-17 15:23:32.000000 platinumtools-0.4.1/test_scenarios/test_scheduling.py
```

### Comparing `platinumtools-0.4/LICENSE` & `platinumtools-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/PKG-INFO` & `platinumtools-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platinumtools
-Version: 0.4
+Version: 0.4.1
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `platinumtools-0.4/platinumtools/aws_classes/CommonProcesor.py` & `platinumtools-0.4.1/platinumtools/aws_classes/CommonProcesor.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/platinumtools/aws_classes/JobListener.py` & `platinumtools-0.4.1/platinumtools/aws_classes/JobListener.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/platinumtools/aws_classes/class_adapters.py` & `platinumtools-0.4.1/platinumtools/aws_classes/class_adapters.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/platinumtools/aws_classes/class_enhancement.py` & `platinumtools-0.4.1/platinumtools/aws_classes/class_enhancement.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,26 +133,26 @@
                 if len(interactions.keys()) > 0:
                     return "ACTIVE"
                 else:
                     return "PASSIVE"
 
             # Receive data regarding the span guid
             span_guid = event["spanId"] if "spanId" in event else ""
-            event_endtime = event["endTime"] if "endTime" in event else event["timestamp_utc"]
+            event_timestamp = event["timestamp_utc"] if "timestamp_utc" in event else event["timestamp"] if "timestamp" in event else None, #Always
+            event_endtime = event["endTime"] if "endTime" in event else event_timestamp
             event_duration = event["duration"] if "duration" in event else 0
             
             # Receive data regarding the span guid from the Organization Querier using isRootOrUpdateRoot
             
             # In form of {is_root: bool, total_duration: number, root_reference: str}
             
             span_guid_data = self.organizationalQuerier.isRootOrUpdateRoot(span_guid=span_guid, event_endtime=event_endtime, event_duration=event_duration )
             is_root = span_guid_data["is_root"] # This is the is_root that will be used for the event
             total_duration = span_guid_data["total_duration"] # This is the root_duration that will be used for the event
             root_reference = span_guid_data["root_reference"] # This is the root_reference that will be used for the event
-            event_timestamp = event["timestamp_utc"] if "timestamp_utc" in event else event["tiemstamp"] if "tiemstamp" in event else None, #Always
             # Remeber to null safe all this
             fileEvent = ChromeEvent(
                 event_guid=management_api.organization_guid,
                 employee_guid=organization_params[employee_id]["employee_guid"],
                 timestamp_utc=event_timestamp,
                 loadbatch_id=management_api.guid,
                 raw_details=event,
```

### Comparing `platinumtools-0.4/platinumtools/aws_classes/class_guardian.py` & `platinumtools-0.4.1/platinumtools/aws_classes/class_guardian.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/platinumtools/aws_classes/class_helpers.py` & `platinumtools-0.4.1/platinumtools/aws_classes/class_helpers.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/platinumtools/aws_classes/class_scheduling.py` & `platinumtools-0.4.1/platinumtools/aws_classes/class_scheduling.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/platinumtools/aws_classes/config_mapper.py` & `platinumtools-0.4.1/platinumtools/aws_classes/config_mapper.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/platinumtools/aws_classes/config_mapper_df.py` & `platinumtools-0.4.1/platinumtools/aws_classes/config_mapper_df.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/platinumtools/dda_constants.py` & `platinumtools-0.4.1/platinumtools/dda_constants.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/platinumtools/dda_models.py` & `platinumtools-0.4.1/platinumtools/dda_models.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/platinumtools.egg-info/PKG-INFO` & `platinumtools-0.4.1/platinumtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platinumtools
-Version: 0.4
+Version: 0.4.1
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `platinumtools-0.4/platinumtools.egg-info/SOURCES.txt` & `platinumtools-0.4.1/platinumtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/setup.py` & `platinumtools-0.4.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.4'
+VERSION = '0.4.1'
 DESCRIPTION = 'DDAPP Modules'
 LONG_DESCRIPTION = 'Common Constants, classes and methods for ETL and other python projects'
 
 # Setting up
 #nenewang08
 setup(
     name="platinumtools",
```

### Comparing `platinumtools-0.4/test_scenarios/JobListener.py` & `platinumtools-0.4.1/test_scenarios/JobListener.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/test_scenarios/test_adapters.py` & `platinumtools-0.4.1/test_scenarios/test_adapters.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/test_scenarios/test_common_processing.py` & `platinumtools-0.4.1/test_scenarios/test_common_processing.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/test_scenarios/test_enhancement.py` & `platinumtools-0.4.1/test_scenarios/test_enhancement.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/test_scenarios/test_event_normalization.py` & `platinumtools-0.4.1/test_scenarios/test_event_normalization.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/test_scenarios/test_guardian.py` & `platinumtools-0.4.1/test_scenarios/test_guardian.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/test_scenarios/test_helpers.py` & `platinumtools-0.4.1/test_scenarios/test_helpers.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.4/test_scenarios/test_scheduling.py` & `platinumtools-0.4.1/test_scenarios/test_scheduling.py`

 * *Files identical despite different names*

