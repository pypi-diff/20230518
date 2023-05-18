# Comparing `tmp/rapidpe_rift_pipe-0.2.3.dev20230518.tar.gz` & `tmp/rapidpe_rift_pipe-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.2.3.dev20230518.tar", last modified: Thu May 18 05:16:27 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.3.0.tar", last modified: Thu May 18 20:48:49 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.2.3.dev20230518.tar` & `rapidpe_rift_pipe-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 05:16:27.737044 rapidpe_rift_pipe-0.2.3.dev20230518/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1140 2023-05-18 05:16:27.737044 rapidpe_rift_pipe-0.2.3.dev20230518/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 05:16:27.728043 rapidpe_rift_pipe-0.2.3.dev20230518/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 05:16:27.730044 rapidpe_rift_pipe-0.2.3.dev20230518/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5579 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1449 2023-05-18 05:16:27.776045 rapidpe_rift_pipe-0.2.3.dev20230518/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 05:16:27.728043 rapidpe_rift_pipe-0.2.3.dev20230518/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 05:16:27.734044 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    38011 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18297 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 05:16:27.736044 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 05:16:09.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 05:16:27.736044 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 05:16:09.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31226 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    27658 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 05:16:27.737044 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 05:16:09.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 05:16:27.735044 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1140 2023-05-18 05:16:27.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-05-18 05:16:27.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 05:16:27.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-18 05:16:27.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-05-18 05:16:27.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-18 05:16:27.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 05:16:27.000000 rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.696423 rapidpe_rift_pipe-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-18 20:48:49.696423 rapidpe_rift_pipe-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.515417 rapidpe_rift_pipe-0.3.0/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.518417 rapidpe_rift_pipe-0.3.0/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5579 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-18 20:48:49.698423 rapidpe_rift_pipe-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.515417 rapidpe_rift_pipe-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.685423 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-18 20:44:54.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    40087 2023-05-18 18:03:43.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18503 2023-05-18 18:03:43.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.693423 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 20:48:33.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.694423 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 20:48:33.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31226 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    27658 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.696423 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 20:48:33.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.693423 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/COPYING` & `rapidpe_rift_pipe-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/PKG-INFO` & `rapidpe_rift_pipe-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.2.3.dev20230518
+Version: 0.3.0
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.3.0/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.3.0/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.3.0/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.3.0/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.3.0/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/setup.cfg` & `rapidpe_rift_pipe-0.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -49,10 +49,10 @@
 rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = dev.20230518
+tag_build = 
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,37 @@
 @lsctables.use_in
 class LIGOLWContentHandler(ligolw.LIGOLWContentHandler):
     pass
 
 
 _allowed_pipelines = ["gstlal", "spiir", "MBTAOnline"]
 
+# Default channels from: https://wiki.ligo.org/LSC/JRPComm/ObsRun3
+# TODO: Add K1 and offline channel names from:
+#       https://wiki.ligo.org/LSC/JRPComm/ObsRun4
+# TODO: Do this more programmatically.  Data isn't in GraceDB, but maybe is
+#       accessible from GWDataFind?
+_run_mode_to_channels = {
+    "online": {
+        "H1": "GDS-CALIB_STRAIN_CLEAN",
+        "L1": "GDS-CALIB_STRAIN_CLEAN",
+        "V1": "Hrec_hoft_16384Hz",
+    },
+    "o2replay": {
+        "H1": "GDS-CALIB_STRAIN_O2Replay",
+        "L1": "GDS-CALIB_STRAIN_O2Replay",
+        "V1": "Hrec_hoft_16384Hz_O2Replay",
+    },
+    "o3replay": {
+        "H1": "GDS-CALIB_STRAIN_INJ1_O3Replay",
+        "L1": "GDS-CALIB_STRAIN_INJ1_O3Replay",
+        "V1": "Hrec_hoft_16384Hz_INJ1_O3Replay",
+    },
+}
+
 
 def make_parser():
     parser = ArgumentParser()
 
     parser.add_argument(
         "config",
         help="Configuration file.",
@@ -309,23 +332,51 @@
         if is_event:
             coinc_xml_filename = os.path.join(output_dir, "coinc.xml")
             # The PSD file name is set here, but it's written later because
             # sometimes it takes a while for the file to upload
             psd_filename = os.path.join(output_dir, "psd.xml.gz")
             skymap_filename = os.path.join(output_dir, "bayestar.fits")
 
+            # If not pulling the channel names from GraceDB, get the dict
+            # mapping IFO -> channel name
+            if config.event.run_mode != "gracedb":
+                ifo_to_channel = _run_mode_to_channels[config.event.run_mode]
+
             # Now, based on the event_time, find the frame files you want.
             channel_str = "["
             psd_file_str = "["
+            num_ifos = 0
             for insp in insp_type["SingleInspiral"]:
-                channel = insp["channel"]
                 ifo = insp["ifo"]
+                logging.info("IFO: %s", ifo)
+
+                if config.event.run_mode == "gracedb":
+                    # Get the channel name from GraceDB
+                    channel = insp["channel"]
+                else:
+                    try:
+                        # Get the channel name based on the hard-coded value
+                        # for the IFO.
+                        channel = ifo_to_channel[ifo]
+                    except KeyError:
+                        # No hard coded value found.  This might happen if a
+                        # new IFO (e.g., K1) is added without us hard-coding
+                        # it.
+                        logging.warning(
+                            "Could not find channel name for IFO `%s' in run "
+                            "mode `%s'.  Skipping `%s'",
+                            ifo, config.event.run_mode, ifo,
+                        )
+                        continue
+
+                logging.info("Channel: %s", channel)
+
                 channel_str += f"{ifo}={channel},"
                 psd_file_str += f"{ifo}={psd_filename},"
-                logging.info("IFO: %s", ifo)
+
                 # Copied from Richards code
                 # https://git.ligo.org/richard-oshaughnessy/research-projects-RIT/blob/temp-RIT-Tides-port_master-GPUIntegration/MonteCarloMarginalizeCode/Code/helper_LDG_Events.py
                 # Estimate signal duration
                 t_event = insp["end_time"]
                 P = lalsimutils.ChooseWaveformParams()
                 P.m1 = insp["mass1"]*lal.MSUN_SI
                 P.m2 = insp["mass2"]*lal.MSUN_SI
@@ -359,14 +410,19 @@
                 )
                 logging.info(dcmd)
                 exit_status = os.system(dcmd)
                 if exit_status != 0:
                     logging.error(dcmd)
                     sys.exit(f"ERROR: non zero exit status {exit_status}")
 
+                num_ifos += 1
+
+            if num_ifos == 0:
+                logging.error("Failed to load data from any IFOs.")
+
             # path2cache always assumes data is in output_dir, so that path
             # needs to be removed before passing output to data.cache
             text_for_sed_removal = "localhost{}\/file:\\/".format(
                 init_directory.replace('/', '\\/')
             )
             if shutil.which('lal_path2cache') is not None:
                 path2cache = 'lal_path2cache'
```

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,27 +426,35 @@
 
 
 _event_group_spec = {
     "gid" : {
         "gracedb_id" : {
             "parser" : parse_str,
         },
+        "run_mode" : {
+            "parser" : parse_str,
+            "fallback" : "online",
+        },
         "mdc_event_injection_file" : {
             "parser": parse_str,
             "fallback": None
         },
         "mdc_time_offset" : {
             "parser" : parse_str,
             "fallback" : None
         },
     },
     "sid" : {
         "superevent_id" : {
             "parser" : parse_str,
         },
+        "run_mode" : {
+            "parser" : parse_str,
+            "fallback" : "online",
+        },
         "mdc_event_injection_file" : {
             "parser": parse_str,
             "fallback": None
         },
         "mdc_time_offset" : {
             "parser" : parse_str,
             "fallback" : None
```

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.2.3.dev20230518
+Version: 0.3.0
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.2.3.dev20230518/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

