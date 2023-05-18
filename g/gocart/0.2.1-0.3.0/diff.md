# Comparing `tmp/gocart-0.2.1.tar.gz` & `tmp/gocart-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocart-0.2.1.tar", last modified: Wed Apr 26 18:36:08 2023, max compression
+gzip compressed data, was "gocart-0.3.0.tar", last modified: Thu May 18 20:22:09 2023, max compression
```

## Comparing `gocart-0.2.1.tar` & `gocart-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.053192 gocart-0.2.1/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1545 2023-04-26 18:31:54.000000 gocart-0.2.1/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-04-26 18:31:54.000000 gocart-0.2.1/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-04-26 18:31:54.000000 gocart-0.2.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-26 18:36:08.053192 gocart-0.2.1/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5430 2023-04-26 18:31:54.000000 gocart-0.2.1/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.049192 gocart-0.2.1/gocart/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/advanced_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8322 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.049192 gocart-0.2.1/gocart/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1920 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/commonutils/flatten_healpix_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2956 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/commonutils/generate_skymap_stats.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/commonutils/getpackagepath.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.053192 gocart-0.2.1/gocart/convert/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/convert/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12416 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/convert/aitoff.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3293 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/convert/ascii.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/convert/healpix2cart.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3033 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.053192 gocart-0.2.1/gocart/parsers/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/parsers/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13302 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/parsers/lvk.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2770 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-04-26 18:31:54.000000 gocart-0.2.1/gocart/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-26 18:36:08.049192 gocart-0.2.1/gocart.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5996 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      748 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-26 18:35:09.000000 gocart-0.2.1/gocart.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      113 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-04-26 18:36:07.000000 gocart-0.2.1/gocart.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-04-26 18:36:08.053192 gocart-0.2.1/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1934 2023-04-26 18:31:54.000000 gocart-0.2.1/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.842508 gocart-0.3.0/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2071 2023-05-18 20:17:14.000000 gocart-0.3.0/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-05-18 20:17:14.000000 gocart-0.3.0/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-05-18 20:17:14.000000 gocart-0.3.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6065 2023-05-18 20:22:09.842508 gocart-0.3.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5499 2023-05-18 20:17:14.000000 gocart-0.3.0/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.834508 gocart-0.3.0/gocart/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8730 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.838508 gocart-0.3.0/gocart/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1920 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/commonutils/flatten_healpix_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/commonutils/generate_skymap_stats.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/commonutils/getpackagepath.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.838508 gocart-0.3.0/gocart/convert/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/convert/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12423 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/convert/aitoff.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3420 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/convert/ascii.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/convert/healpix2cart.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3033 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/default_settings.yaml
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.838508 gocart-0.3.0/gocart/parsers/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/parsers/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14405 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/parsers/lvk.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.806507 gocart-0.3.0/gocart/resources/
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.842508 gocart-0.3.0/gocart/resources/plugins/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-05-18 20:17:15.000000 gocart-0.3.0/gocart/resources/plugins/gp_template.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-05-18 20:17:15.000000 gocart-0.3.0/gocart/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2770 2023-05-18 20:17:15.000000 gocart-0.3.0/gocart/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-05-18 20:17:15.000000 gocart-0.3.0/gocart/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.834508 gocart-0.3.0/gocart.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6065 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      788 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-18 20:20:59.000000 gocart-0.3.0/gocart.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      113 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-05-18 20:22:09.842508 gocart-0.3.0/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1934 2023-05-18 20:17:15.000000 gocart-0.3.0/setup.py
```

### Comparing `gocart-0.2.1/CHANGES.md` & `gocart-0.3.0/CHANGES.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 
 ## Release Notes
 
+**v0.3.0 - May 18, 2023**  
+
+- **FEATURE**: user can now add their own plugin scripts to run every time an alert is parsed  
+- **ENHANCEMENT**: added a count of alerts read when first connected to kafka (gives users peace of mind that goacrt is working)  
+- **FIXED**: area calulations fixed (I was still sort by prob but should have been sorting by probdensity for mulit-order maps)  
+- **FIXED**: can still read an event ID even if not found in the sky-map header (tried to find the event ID from the map directory path)  
+
 **v0.2.1 - April 26, 2023**  
 
 - **FIXED**: listen command was tripping up on mock-events
 
 **v0.2.0 - April 26, 2023**  
 
 - **FEATURE**: filtering of alerts is now possible via options in the settings file (see docs)
```

### Comparing `gocart-0.2.1/LICENSE` & `gocart-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gocart-0.2.1/PKG-INFO` & `gocart-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.2.1
+Version: 0.3.0
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.2.1.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.3.0.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
@@ -39,14 +39,15 @@
 
 ## Features
 
 - Listen to GCN Kafka streams (currently  LIGO-Virgo-KAGRA only) and write alerts and skymaps to the local filesystem.
 - Ability to 'echo' the Kafka stream by re-listening to the last N days of alerts (provided the alerts are still hosted on the GCN Kafka cluster).
 - Alert content, FITS Header data and some extra value-added event parameters are written to a single machine-readable YAML file.
 - The healpix skymaps are optionally converted to ascii files (one row per healpix pixel) and/or rendered as aitoff plots.
+- Create your own plugin scripts to run whenever an alert is parsed.
 
 
 ## Installation
 
 The easiest way to install gocart is to use `conda`:
 
 ``` bash
```

### Comparing `gocart-0.2.1/README.md` & `gocart-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 ## Features
 
 - Listen to GCN Kafka streams (currently  LIGO-Virgo-KAGRA only) and write alerts and skymaps to the local filesystem.
 - Ability to 'echo' the Kafka stream by re-listening to the last N days of alerts (provided the alerts are still hosted on the GCN Kafka cluster).
 - Alert content, FITS Header data and some extra value-added event parameters are written to a single machine-readable YAML file.
 - The healpix skymaps are optionally converted to ascii files (one row per healpix pixel) and/or rendered as aitoff plots.
+- Create your own plugin scripts to run whenever an alert is parsed.
 
 
 ## Installation
 
 The easiest way to install gocart is to use `conda`:
 
 ``` bash
```

### Comparing `gocart-0.2.1/gocart/advanced_settings.yaml` & `gocart-0.3.0/gocart/advanced_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.2.1/gocart/cl_utils.py` & `gocart-0.3.0/gocart/cl_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 #!/usr/bin/env python
 # encoding: utf-8
 """
 Documentation for gocart can be found here: http://gocart.readthedocs.org
 
 Usage:
     gocart init
-    gocart echo <daysAgo> [-s <pathToSettingsFile>]
-    gocart listen [-s <pathToSettingsFile>]
+    gocart [-p] echo <daysAgo> [-s <pathToSettingsFile>]
+    gocart [-p] listen [-s <pathToSettingsFile>]
 
 
 Options:
     init                                   setup the gocart settings file for the first time
     echo <daysAgo>                         relisten to alerts from N <daysAgo> until now and then exit
     listen                                 reconnect to kafka stream and listen from where you left off (or from now on if connectiong for the first time).
 
     -h, --help                             show this help message
     -v, --version                          show version
+    -p, --plugins                          execute plugins everytime an alert is read
     -s, --settings <pathToSettingsFile>    the settings file
     -t, --test                             test, only collect 1 map
 """
 from subprocess import Popen, PIPE, STDOUT
 from fundamentals import tools, times
 from docopt import docopt
 import pickle
 import glob
 import readline
 import sys
 import os
+import shutil
 os.environ['TERM'] = 'vt100'
 
 
 def tab_complete(text, state):
     return (glob.glob(text + '*') + [None])[state]
 
 
@@ -89,31 +91,27 @@
 
     ## START LOGGING ##
     startTime = times.get_now_sql_datetime()
     log.info(
         '--- STARTING TO RUN THE cl_utils.py AT %s' %
         (startTime,))
 
+    # TEST IF PLUG FOLDER EXISTS
+    from os.path import expanduser
+    home = expanduser("~")
+    pluginPath = home + "/.config/gocart/plugins"
+    exists = os.path.exists(pluginPath)
+    if not exists:
+        shutil.copytree(os.path.dirname(__file__) + "/resources/plugins", pluginPath)
+
     if a["init"]:
         from os.path import expanduser
         home = expanduser("~")
         filepath = home + "/.config/gocart/gocart.yaml"
 
-        try:
-            cmd = """open %(filepath)s""" % locals()
-            p = Popen(cmd, stdout=PIPE, stderr=PIPE, shell=True)
-        except:
-            pass
-        try:
-            cmd = """start %(filepath)s""" % locals()
-            p = Popen(cmd, stdout=PIPE, stderr=PIPE, shell=True)
-        except:
-            pass
-        return
-
     topic = 'igwn.gwalert'
 
     if len(settings['gcn-kafka']['client_id']) < 6 or len(settings['gcn-kafka']['client_secret']) < 6:
         print("Please add your gcn-kafka client ID and secret to the gocart.yaml settings file.")
         return
 
     if a['listen'] or a['echo']:
@@ -166,31 +164,37 @@
         stop = False
         test = 0
         more = True
         while not stop:
             # IF FISRT TIME CONNECTING THEN SKIP MESSAGES
             if firstConnect:
                 count = 0
-                print("Marking previous messages as read, this can take a few minutes ...")
+                index = 1
+                print("Marking previous messages as read, this can take a few minutes")
                 while more:
-                    messages = consumer.consume(num_messages=300, timeout=10)
-
+                    messages = consumer.consume(num_messages=300, timeout=5)
                     for message in messages:
                         count += 1
                         consumer.commit(message)
+                    if index > 1:
+                        # Cursor up one line and clear line
+                        sys.stdout.write("\x1b[1A\x1b[2K")
+                    index += 1
+                    print(f"{count} messages read ...")
                     if not len(messages):
                         more = False
 
                 firstConnect = False
                 print(f"This is your first time using the listen command. gocart will now listen for all new incoming alerts (skipping the {count} previous alerts currently in this topic). If you stop listening and restart sometime later, gocart will immediately collect all alerts missed while off-line.")
             for message in consumer.consume(timeout=1):
                 parser = lvk(
                     log=log,
                     record=message.value(),
-                    settings=settings
+                    settings=settings,
+                    plugins=a["pluginsFlag"]
                 ).parse()
                 consumer.commit(message)
 
     if a['echo'] and a['daysAgo']:
         # GET MESSAGES OCCURRING IN LAST N DAYS
         from gcn_kafka import Consumer
         from confluent_kafka import TopicPartition
@@ -213,15 +217,16 @@
         more = True
         while more:
             messages = consumer.consume(num_messages=1, timeout=10)
             for message in messages:
                 parser = lvk(
                     log=log,
                     record=message.value(),
-                    settings=settings
+                    settings=settings,
+                    plugins=a["pluginsFlag"]
                 ).parse()
             if not len(messages):
                 more = False
 
     ## FINISH LOGGING ##
     endTime = times.get_now_sql_datetime()
     runningTime = times.calculate_time_difference(startTime, endTime)
```

### Comparing `gocart-0.2.1/gocart/commonutils/flatten_healpix_map.py` & `gocart-0.3.0/gocart/commonutils/flatten_healpix_map.py`

 * *Files identical despite different names*

### Comparing `gocart-0.2.1/gocart/commonutils/generate_skymap_stats.py` & `gocart-0.3.0/gocart/commonutils/generate_skymap_stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,26 +52,28 @@
     tableData['NSIDE'] = ah.level_to_nside(tableData['LEVEL'])
     # DETERMINE THE PIXEL AREA AND PROB OF EACH PIXEL
     tableData['AREA'] = ah.nside_to_pixel_area(tableData['NSIDE']).to_value(u.steradian)
     tableData['PROB'] = tableData['AREA'] * tableData["PROBDENSITY"]
     tableData['AREA'] = ah.nside_to_pixel_area(tableData['NSIDE']).to_value(u.deg**2)
 
     # SORT BY PROB, CALCULATE CUMULATIVE PROB AND RESORT BY INDEX
-    tableData.sort_values(["PROB"],
+    tableData.sort_values(["PROBDENSITY"],
                           ascending=[False], inplace=True)
     tableData["CUMPROB"] = np.cumsum(tableData['PROB'])
 
     # FILTER DATA FRAME
     # FIRST CREATE THE MASK
     mask = (tableData["CUMPROB"] < 0.9)
     area90 = tableData.loc[mask, 'AREA'].sum()
     mask = (tableData["CUMPROB"] < 0.5)
     area50 = tableData.loc[mask, 'AREA'].sum()
     mask = (tableData["CUMPROB"] < 0.1)
     area10 = tableData.loc[mask, 'AREA'].sum()
+    mask = (tableData["CUMPROB"] < 0.99999999999999)
+    area100 = tableData['AREA'].sum()
 
     area90 = float(f'{area90:.3f}')
     area50 = float(f'{area50:.3f}')
     area10 = float(f'{area10:.3f}')
 
     extras = {"area90": area90, "area50": area50, "area10": area10}
```

### Comparing `gocart-0.2.1/gocart/convert/aitoff.py` & `gocart-0.3.0/gocart/convert/aitoff.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             planeColour = "#dc322f"
             ax.scatter(np.radians(gx), np.radians(gDec),
                        color=planeColour, alpha=1, s=1)
             line = Line2D([0], [0], label='Galactic Plane', color=planeColour)
             handles.append(line)
 
         if contours:
-            mapDF.sort_values(["PROB"],
+            mapDF.sort_values(["PROBDENSITY"],
                               ascending=[False], inplace=True)
             mapDF["CUMPROB"] = np.cumsum(mapDF['PROB'])
             mapDF["CUMPROB"] = mapDF["CUMPROB"] * 100. * mapDF["PROB"].sum()
             mapDF.sort_index(inplace=True)
             contours = mapDF["CUMPROB"].values.reshape((ysize, xsize))
 
             colors = ['#474973', '#a69cac', '#03F7EB']
```

### Comparing `gocart-0.2.1/gocart/convert/ascii.py` & `gocart-0.3.0/gocart/convert/ascii.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,15 +99,19 @@
         # DROP COLUMNS
         try:
             tableData.drop(columns=['DISTNORM'], inplace=True)
         except:
             pass
 
         # CREATE HEADER FOR FILE
-        header = f"# EVENT:{self.table.meta['objid']}\n"
+        try:
+            header = f"# EVENT:{self.table.meta['objid']}\n"
+        except:
+            eventId = self.mapPath.split("/")[-3]
+            header = f"# EVENT:{eventId}\n"
         header += f"# NSIDE:{self.nside}\n"
 
         tableData.index.names = ['IPIX']
         asciiContent = tableData.to_csv(index=True)
         asciiContent = header + asciiContent
 
         if outputFilepath:
```

### Comparing `gocart-0.2.1/gocart/convert/healpix2cart.py` & `gocart-0.3.0/gocart/convert/healpix2cart.py`

 * *Files identical despite different names*

### Comparing `gocart-0.2.1/gocart/default_settings.yaml` & `gocart-0.3.0/gocart/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.2.1/gocart/parsers/lvk.py` & `gocart-0.3.0/gocart/parsers/lvk.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,45 +22,49 @@
     """
     *The LVK event parser*
 
     **Key Arguments:**
         - ``log`` -- logger
         - ``settings`` -- the settings dictionary
         - ``record`` -- the kafka record to parse.
+        - ``plugins`` -- run the plugin script found in `~/.config/gocart/plugins` every time an alert is read
 
     **Usage:**
 
     To setup your logger and settings, please use the ``fundamentals`` package (`see tutorial here <http://fundamentals.readthedocs.io/en/latest/#tutorial>`_).
 
     To parse LVK kafka alerts, use the following:
 
     ```python
     from gocart.parsers import lvk
     parser = lvk(
         log=log,
         record=record,
-        settings=settings
+        settings=settings,
+        plugins=True
     ).parse()
     ```
 
     """
 
     def __init__(
             self,
             log,
             record,
             settings=False,
+            plugins=False
 
     ):
         import json
 
         self.log = log
         log.debug("instansiating a new 'lvk' object")
         self.settings = settings
         self.record = json.loads(record)
+        self.plugins = plugins
 
         import inspect
         import yaml
         # COLLECT ADVANCED SETTINGS IF AVAILABLE
         parentDirectory = os.path.dirname(__file__)
         advs = parentDirectory + "/advanced_settings.yaml"
         level = 0
@@ -249,14 +253,32 @@
                     meta=meta
                 )
                 c.convert(
                     galacticPlane=self.settings["lvk"]["aitoff"]["galactic_plane"],
                     sunmoonContour=self.settings["lvk"]["aitoff"]["sun_moon_contour"],
                     sunmoon=self.settings["lvk"]["aitoff"]["sun_moon"])
 
+        if self.plugins:
+            from os.path import expanduser
+            from subprocess import Popen, PIPE, STDOUT
+            home = expanduser("~")
+            # GENERATE A LIST OF FILE PATHS
+            pathToDirectory = home + "/.config/gocart/plugins"
+            for d in os.listdir(pathToDirectory):
+                filepath = os.path.join(pathToDirectory, d)
+                if os.path.isfile(filepath) and d[:3] == "gp_":
+                    cmd = f"""/usr/bin/env python {filepath} {alertDir}"""
+                    print(f"PLUGIN: {d}")
+                    try:
+                        p = Popen(cmd, stdout=PIPE, stderr=PIPE, shell=True)
+                        stdout, stderr = p.communicate()
+                        print(stdout.decode('utf-8'))
+                    except Exception as e:
+                        self.log.error(f'cound not execute the {d} plugin. Failed with error: {e}')
+
         self.log.debug('completed the ``parse`` method')
         return lvk
 
     def filter_alert(
             self,
             alert):
         """*filter the alert record with filtering criteria in the settings file and return true (pass) or false (fail)*
```

### Comparing `gocart-0.2.1/gocart/setup.cfg` & `gocart-0.3.0/gocart/setup.cfg`

 * *Files identical despite different names*

### Comparing `gocart-0.2.1/gocart/test_settings.yaml` & `gocart-0.3.0/gocart/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.2.1/gocart/utKit.py` & `gocart-0.3.0/gocart/utKit.py`

 * *Files identical despite different names*

### Comparing `gocart-0.2.1/gocart.egg-info/PKG-INFO` & `gocart-0.3.0/gocart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.2.1
+Version: 0.3.0
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.2.1.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.3.0.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
@@ -39,14 +39,15 @@
 
 ## Features
 
 - Listen to GCN Kafka streams (currently  LIGO-Virgo-KAGRA only) and write alerts and skymaps to the local filesystem.
 - Ability to 'echo' the Kafka stream by re-listening to the last N days of alerts (provided the alerts are still hosted on the GCN Kafka cluster).
 - Alert content, FITS Header data and some extra value-added event parameters are written to a single machine-readable YAML file.
 - The healpix skymaps are optionally converted to ascii files (one row per healpix pixel) and/or rendered as aitoff plots.
+- Create your own plugin scripts to run whenever an alert is parsed.
 
 
 ## Installation
 
 The easiest way to install gocart is to use `conda`:
 
 ``` bash
```

### Comparing `gocart-0.2.1/gocart.egg-info/SOURCES.txt` & `gocart-0.3.0/gocart.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 gocart/commonutils/generate_skymap_stats.py
 gocart/commonutils/getpackagepath.py
 gocart/convert/__init__.py
 gocart/convert/aitoff.py
 gocart/convert/ascii.py
 gocart/convert/healpix2cart.py
 gocart/parsers/__init__.py
-gocart/parsers/lvk.py
+gocart/parsers/lvk.py
+gocart/resources/plugins/gp_template.py
```

### Comparing `gocart-0.2.1/setup.py` & `gocart-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open(moduleDirectory + '/README.md') as f:
         return f.read()
 
 
 install_requires = [
     'pyyaml',
     'fundamentals',
-    'astropy==5.1.0',
+    'astropy==5.2.0',
     'astropy-healpix',
     'numpy',
     'matplotlib',
     'healpy',
     'pandas',
     'tabulate',
     'ligo.skymap',
```

