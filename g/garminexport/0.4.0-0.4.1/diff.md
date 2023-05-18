# Comparing `tmp/garminexport-0.4.0.tar.gz` & `tmp/garminexport-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garminexport-0.4.0.tar", last modified: Sun May  9 06:19:34 2021, max compression
+gzip compressed data, was "garminexport-0.4.1.tar", last modified: Fri Mar 18 16:32:38 2022, max compression
```

## Comparing `garminexport-0.4.0.tar` & `garminexport-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)        0 2021-05-09 06:19:34.815882 garminexport-0.4.0/
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)    11325 2021-05-09 05:22:59.000000 garminexport-0.4.0/LICENSE
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     7225 2021-05-09 06:19:34.815882 garminexport-0.4.0/PKG-INFO
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     5166 2021-05-09 05:22:59.000000 garminexport-0.4.0/README.md
-drwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)        0 2021-05-09 06:19:34.811882 garminexport-0.4.0/garminexport/
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)        0 2021-05-09 05:22:59.000000 garminexport-0.4.0/garminexport/__init__.py
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     7140 2021-05-09 05:22:59.000000 garminexport-0.4.0/garminexport/backup.py
-drwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)        0 2021-05-09 06:19:34.815882 garminexport-0.4.0/garminexport/cli/
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)        0 2021-05-09 05:22:59.000000 garminexport-0.4.0/garminexport/cli/__init__.py
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     3822 2021-05-09 06:02:56.000000 garminexport-0.4.0/garminexport/cli/backup.py
--rwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)     3123 2021-05-09 05:22:59.000000 garminexport-0.4.0/garminexport/cli/get_activity.py
--rwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)     2765 2021-05-09 05:22:59.000000 garminexport-0.4.0/garminexport/cli/upload_activity.py
--rwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)    22418 2021-05-09 06:07:19.000000 garminexport-0.4.0/garminexport/garminclient.py
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     3916 2021-05-09 06:07:43.000000 garminexport-0.4.0/garminexport/incremental_backup.py
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)      224 2021-05-09 05:22:59.000000 garminexport-0.4.0/garminexport/logging_config.py
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     8151 2021-05-09 05:22:59.000000 garminexport-0.4.0/garminexport/retryer.py
-drwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)        0 2021-05-09 06:19:34.811882 garminexport-0.4.0/garminexport.egg-info/
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     7225 2021-05-09 06:19:34.000000 garminexport-0.4.0/garminexport.egg-info/PKG-INFO
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)      551 2021-05-09 06:19:34.000000 garminexport-0.4.0/garminexport.egg-info/SOURCES.txt
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)        1 2021-05-09 06:19:34.000000 garminexport-0.4.0/garminexport.egg-info/dependency_links.txt
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)      184 2021-05-09 06:19:34.000000 garminexport-0.4.0/garminexport.egg-info/entry_points.txt
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)       38 2021-05-09 06:19:34.000000 garminexport-0.4.0/garminexport.egg-info/requires.txt
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)       13 2021-05-09 06:19:34.000000 garminexport-0.4.0/garminexport.egg-info/top_level.txt
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)      100 2021-05-09 05:23:48.000000 garminexport-0.4.0/pyproject.toml
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)       38 2021-05-09 06:19:34.815882 garminexport-0.4.0/setup.cfg
--rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     2240 2021-05-09 06:18:35.000000 garminexport-0.4.0/setup.py
+drwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)        0 2022-03-18 16:32:38.705524 garminexport-0.4.1/
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)    11325 2021-05-09 05:22:59.000000 garminexport-0.4.1/LICENSE
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     7232 2022-03-18 16:32:38.705524 garminexport-0.4.1/PKG-INFO
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     6111 2022-03-18 16:26:23.000000 garminexport-0.4.1/README.md
+drwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)        0 2022-03-18 16:32:38.705524 garminexport-0.4.1/garminexport/
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)        0 2021-05-09 05:22:59.000000 garminexport-0.4.1/garminexport/__init__.py
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     7140 2021-05-09 05:22:59.000000 garminexport-0.4.1/garminexport/backup.py
+drwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)        0 2022-03-18 16:32:38.705524 garminexport-0.4.1/garminexport/cli/
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)        0 2021-05-09 05:22:59.000000 garminexport-0.4.1/garminexport/cli/__init__.py
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     3822 2021-05-09 06:02:56.000000 garminexport-0.4.1/garminexport/cli/backup.py
+-rwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)     3123 2021-05-09 05:22:59.000000 garminexport-0.4.1/garminexport/cli/get_activity.py
+-rwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)     2765 2021-05-09 05:22:59.000000 garminexport-0.4.1/garminexport/cli/upload_activity.py
+-rwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)    22806 2022-03-18 16:26:23.000000 garminexport-0.4.1/garminexport/garminclient.py
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     3916 2021-05-09 06:07:43.000000 garminexport-0.4.1/garminexport/incremental_backup.py
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)      224 2021-05-09 05:22:59.000000 garminexport-0.4.1/garminexport/logging_config.py
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     8151 2021-05-09 05:22:59.000000 garminexport-0.4.1/garminexport/retryer.py
+drwxrwxr-x   0 pgwrk     (1003) pgwrk     (1003)        0 2022-03-18 16:32:38.705524 garminexport-0.4.1/garminexport.egg-info/
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     7232 2022-03-18 16:32:37.000000 garminexport-0.4.1/garminexport.egg-info/PKG-INFO
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)      551 2022-03-18 16:32:38.000000 garminexport-0.4.1/garminexport.egg-info/SOURCES.txt
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)        1 2022-03-18 16:32:37.000000 garminexport-0.4.1/garminexport.egg-info/dependency_links.txt
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)      183 2022-03-18 16:32:38.000000 garminexport-0.4.1/garminexport.egg-info/entry_points.txt
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)       70 2022-03-18 16:32:38.000000 garminexport-0.4.1/garminexport.egg-info/requires.txt
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)       13 2022-03-18 16:32:38.000000 garminexport-0.4.1/garminexport.egg-info/top_level.txt
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)      100 2021-05-09 05:23:48.000000 garminexport-0.4.1/pyproject.toml
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)       38 2022-03-18 16:32:38.705524 garminexport-0.4.1/setup.cfg
+-rw-rw-r--   0 pgwrk     (1003) pgwrk     (1003)     2340 2022-03-18 16:27:56.000000 garminexport-0.4.1/setup.py
```

### Comparing `garminexport-0.4.0/LICENSE` & `garminexport-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `garminexport-0.4.0/PKG-INFO` & `garminexport-0.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,140 +1,17 @@
 Metadata-Version: 2.1
 Name: garminexport
-Version: 0.4.0
+Version: 0.4.1
 Summary: Garmin Connect activity exporter and backup tool
 Home-page: https://github.com/petergardfjall/garminexport
 Author: Peter Gardfjäll
 Author-email: peter.gardfjall.work@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/petergardfjall/garminexport.git
 Project-URL: Tracker, https://github.com/petergardfjall/garminexport/issues
-Description: [![Build Status](https://travis-ci.org/petergardfjall/garminexport.svg?branch=master)](https://travis-ci.org/petergardfjall/garminexport)
-        [![PyPi release](https://img.shields.io/pypi/v/garminexport.svg)](https://img.shields.io/pypi/v/garminexport.svg)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/garminexport)
-        ![PyPI - License](https://img.shields.io/pypi/l/garminexport)
-        
-        # About
-        `garminexport` is both a library and a utility script for downloading/backing up
-        [Garmin Connect](http://connect.garmin.com/) activities to a local disk.
-        
-        The main utility script is called `garmin-backup` and performs incremental
-        backups of your Garmin account to a local directory. The first time
-        `garmin-backup` is run, it will download *all* activities. After that, it will
-        do incremental backups of your account. That is, the script will only download
-        activities that haven't already been downloaded to the backup directory.
-        
-        
-        # Installation
-        `garminexport` is available on [PyPi](https://pypi.org/) and can be installed
-        with [pip](http://pip.readthedocs.org):
-        
-            pip install garminexport
-        
-        It requires Python 3.5+.
-        
-        
-        # Usage
-        
-        
-        ## Prerequisites
-        To be of any use you need to register an account at [Garmin
-        Connect](http://connect.garmin.com/) and populate it with some activities.
-        
-        
-        ## As a command-line tool (garmin-backup)
-        
-        The backup program is run as follows (use the `--help` flag for a full list of
-        available options):
-        
-            garmin-backup --backup-dir=activities <username or email>
-        
-        Once started, the program will prompt you for your account password and then log
-        in to your Garmin Connect account to download activities to the specified backup
-        directory on your machine. The program will only download activities that aren't
-        already in the backup directory.
-        
-        Activities can be exported in any of the formats outlined below. Note that
-        by default, the program downloads all formats for every activity. Use the
-        `--format` option to narrow the selection.
-        
-        Supported export formats:
-        
-        
-          -   `gpx`: activity GPX file (XML).
-        
-              <sub>[GPX](https://en.wikipedia.org/wiki/GPS_Exchange_Format) is an open
-              format, mainly for storing GPS routes/tracks. It does support extensions
-              and Garmin appears to annotate the GPS data with, for example, heart-rate
-              and cadence, when available on your device.</sub>
-        
-          -   `tcx`: an activity TCX file (XML).
-              *Note: a `.tcx` file may not always be possible to export, for example
-              if an activity was uploaded in gpx format. In that case, Garmin won't try
-              to synthesize a tcx file.*
-        
-              <sub>[TCX](https://en.wikipedia.org/wiki/Training_Center_XML) (Training
-              Center XML) is Garmin's own XML format. It is, essentially, an extension
-              of GPX which includes more metrics and divides the GPS track into "laps"
-              as recorded by your device (with "lap summaries" for each metric).</sub>
-        
-          -   `fit`: activity FIT file (binary format).
-              *Note: a `.fit` file may not always be possible to export, for example
-              if an activity was entered manually rather than imported from a Garmin device.*
-        
-              <sub>The [FIT](https://www.thisisant.com/resources/fit/) format is the
-              "raw data type" stored in your Garmin device and should contain all
-              metrics your device is capable of tracking (GPS, heart rate, cadence,
-              etc). It's a binary format, so tools are needed to read its content.</sub>
-        
-          -   `json_summary`: activity summary file (JSON).
-        
-              <sub>Provides summary data for an activity. Seems to lack a formal schema
-              and should not be counted on as a stable data format (it may change at any
-              time). Only included since it *may* contain additional data that could be
-              useful for developers of analysis tools.</sub>
-        
-          -   `json_details`: activity details file (JSON).
-        
-              <sub>Provides detailed activity data in a JSON format. Seems to lack a
-              formal schema and should not be counted on as a stable data format (it may
-              change at any time). Only included since it *may* contain additional data
-              that could be useful for developers of analysis tools.</sub>
-        
-        All files are written to the same directory (`activities/` by default).  Each
-        activity file is prefixed by its upload timestamp and its activity id.
-        
-        
-        `garminexport` also contains a few smaller utility programs:
-        
-        - `garmin-get-activity`: download a single Garmin Connect activity. Run with
-          `--help`for more details.
-        - `garmin-upload-activity`: uplad a single Garmin Connect activity file (`.fit`,
-          `.gpx`, or `.tcx`). Run with `--help`for more details.
-        
-        
-        ## As a library
-        
-        To build your own tools around the Garmin Connect API you can import the
-        `garminclient` module. It handles authentication to establish a secure session
-        with Garmin Connect. For example use, have a look at the command-line tools
-        under [garminexport/cli](garminexport/cli).
-        
-        
-        # Contribute
-        
-        To work on the code base you need (besides the basic prerequisites outlined
-        above) to have [pipenv](https://github.com/pypa/pipenv) installed.  Create a
-        `virtualenv` (an isolated development environment) and install the required
-        dependencies like so:
-        
-        
-            make venv
-            # or similarly: pipenv install
-        
 Keywords: garmin export backup
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -142,7 +19,161 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5.*, <4
 Description-Content-Type: text/markdown
+Provides-Extra: cloudflare
+License-File: LICENSE
+
+[![Build Status](https://travis-ci.org/petergardfjall/garminexport.svg?branch=master)](https://travis-ci.org/petergardfjall/garminexport)
+[![PyPi release](https://img.shields.io/pypi/v/garminexport.svg)](https://img.shields.io/pypi/v/garminexport.svg)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/garminexport)
+![PyPI - License](https://img.shields.io/pypi/l/garminexport)
+
+# About
+
+`garminexport` is both a library and a tool for downloading/backing up [Garmin
+Connect](http://connect.garmin.com/) activities to a local disk.
+
+The main utility script is called `garmin-backup` and performs incremental
+backups of your Garmin account to a local directory. The first time
+`garmin-backup` is run, it will download *all* activities. After that, it will
+do incremental backups of your account. That is, the script will only download
+activities that haven't already been downloaded to the backup directory.
+
+
+# Installation
+
+`garminexport` is available on [PyPi](https://pypi.org/) and can be installed
+with [pip](http://pip.readthedocs.org):
+
+``` bash
+pip install garminexport
+```
+
+To install `garminexport` with support to circumvent Cloudflare's bot protection
+(which has been known to impact some users) you can install the module with the
+`cloudflare`
+[extra](https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies) like so:
+
+``` bash
+pip install garminexport[cloudflare]
+```
+
+This replaces the default [requests](https://github.com/psf/requests) library
+with [cloudscraper](https://github.com/VeNoMouS/cloudscraper) for HTTP request.
+
+# Usage
+
+## Prerequisites
+To be of any use you need to register an account at [Garmin
+Connect](http://connect.garmin.com/) and populate it with some activities.
+
+
+## As a command-line tool (garmin-backup)
+
+The backup program is run as follows (use the `--help` flag for a full list of
+available options):
+
+``` bash
+garmin-backup --backup-dir=activities <username or email>
+```
+
+Once started, the program will prompt you for your account password and then log
+in to your Garmin Connect account to download activities to the specified backup
+directory on your machine. The program will only download activities that aren't
+already in the backup directory.
+
+Activities can be exported in any of the formats outlined below. Note that
+by default, the program downloads all formats for every activity. Use the
+`--format` option to narrow the selection.
+
+Supported export formats:
+
+
+  -   `gpx`: activity GPX file (XML).
+
+      <sub>[GPX](https://en.wikipedia.org/wiki/GPS_Exchange_Format) is an open
+      format, mainly for storing GPS routes/tracks. It does support extensions
+      and Garmin appears to annotate the GPS data with, for example, heart-rate
+      and cadence, when available on your device.</sub>
+
+  -   `tcx`: an activity TCX file (XML).
+      *Note: a `.tcx` file may not always be possible to export, for example
+      if an activity was uploaded in gpx format. In that case, Garmin won't try
+      to synthesize a tcx file.*
+
+      <sub>[TCX](https://en.wikipedia.org/wiki/Training_Center_XML) (Training
+      Center XML) is Garmin's own XML format. It is, essentially, an extension
+      of GPX which includes more metrics and divides the GPS track into "laps"
+      as recorded by your device (with "lap summaries" for each metric).</sub>
+
+  -   `fit`: activity FIT file (binary format).
+      *Note: a `.fit` file may not always be possible to export, for example
+      if an activity was entered manually rather than imported from a Garmin device.*
+
+      <sub>The [FIT](https://www.thisisant.com/resources/fit/) format is the
+      "raw data type" stored in your Garmin device and should contain all
+      metrics your device is capable of tracking (GPS, heart rate, cadence,
+      etc). It's a binary format, so tools are needed to read its content.</sub>
+
+  -   `json_summary`: activity summary file (JSON).
+
+      <sub>Provides summary data for an activity. Seems to lack a formal schema
+      and should not be counted on as a stable data format (it may change at any
+      time). Only included since it *may* contain additional data that could be
+      useful for developers of analysis tools.</sub>
+
+  -   `json_details`: activity details file (JSON).
+
+      <sub>Provides detailed activity data in a JSON format. Seems to lack a
+      formal schema and should not be counted on as a stable data format (it may
+      change at any time). Only included since it *may* contain additional data
+      that could be useful for developers of analysis tools.</sub>
+
+All files are written to the same directory (`activities/` by default).  Each
+activity file is prefixed by its upload timestamp and its activity id.
+
+`garminexport` also contains a few smaller utility programs:
+
+- `garmin-get-activity`: download a single Garmin Connect activity. Run with
+  `--help`for more details.
+- `garmin-upload-activity`: uplad a single Garmin Connect activity file (`.fit`,
+  `.gpx`, or `.tcx`). Run with `--help`for more details.
+
+## As a library
+
+To build your own tools around the Garmin Connect API you can import the
+`garminclient` module. It handles authentication to establish a secure session
+with Garmin Connect. For example use, have a look at the command-line tools
+under [garminexport/cli](garminexport/cli).
+
+For example, in your `setup.py`, `setup.cfg`, `pyproject.toml` ([PEP
+631](https://peps.python.org/pep-0631/)) add something like:
+
+``` python
+install_requires=[
+    'garminexport',
+    # also installs 'cloudscraper' as a dependency
+    # 'garminexport[cloudflare]',
+    ...
+]
+```
+
+Note: if you happen to have
+[cloudscraper](https://github.com/VeNoMouS/cloudscraper) on your `PACKAGEPATH`
+`GarminClient` will make use of it whenever it needs to make an HTTP request.
+
+# Contribute
+
+To work on the code base you need (besides the basic prerequisites outlined
+above) to have [pipenv](https://github.com/pypa/pipenv) installed.  Create a
+`virtualenv` (an isolated development environment) and install the required
+dependencies like so:
+
+
+    make venv
+    # or similarly: pipenv install
+
+
```

### Comparing `garminexport-0.4.0/README.md` & `garminexport-0.4.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 [![Build Status](https://travis-ci.org/petergardfjall/garminexport.svg?branch=master)](https://travis-ci.org/petergardfjall/garminexport)
 [![PyPi release](https://img.shields.io/pypi/v/garminexport.svg)](https://img.shields.io/pypi/v/garminexport.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/garminexport)
 ![PyPI - License](https://img.shields.io/pypi/l/garminexport)
 
 # About
-`garminexport` is both a library and a utility script for downloading/backing up
-[Garmin Connect](http://connect.garmin.com/) activities to a local disk.
+
+`garminexport` is both a library and a tool for downloading/backing up [Garmin
+Connect](http://connect.garmin.com/) activities to a local disk.
 
 The main utility script is called `garmin-backup` and performs incremental
 backups of your Garmin account to a local directory. The first time
 `garmin-backup` is run, it will download *all* activities. After that, it will
 do incremental backups of your account. That is, the script will only download
 activities that haven't already been downloaded to the backup directory.
 
 
 # Installation
+
 `garminexport` is available on [PyPi](https://pypi.org/) and can be installed
 with [pip](http://pip.readthedocs.org):
 
-    pip install garminexport
-
-It requires Python 3.5+.
+``` bash
+pip install garminexport
+```
+
+To install `garminexport` with support to circumvent Cloudflare's bot protection
+(which has been known to impact some users) you can install the module with the
+`cloudflare`
+[extra](https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies) like so:
+
+``` bash
+pip install garminexport[cloudflare]
+```
 
+This replaces the default [requests](https://github.com/psf/requests) library
+with [cloudscraper](https://github.com/VeNoMouS/cloudscraper) for HTTP request.
 
 # Usage
 
-
 ## Prerequisites
 To be of any use you need to register an account at [Garmin
 Connect](http://connect.garmin.com/) and populate it with some activities.
 
 
 ## As a command-line tool (garmin-backup)
 
 The backup program is run as follows (use the `--help` flag for a full list of
 available options):
 
-    garmin-backup --backup-dir=activities <username or email>
+``` bash
+garmin-backup --backup-dir=activities <username or email>
+```
 
 Once started, the program will prompt you for your account password and then log
 in to your Garmin Connect account to download activities to the specified backup
 directory on your machine. The program will only download activities that aren't
 already in the backup directory.
 
 Activities can be exported in any of the formats outlined below. Note that
@@ -89,30 +103,43 @@
       formal schema and should not be counted on as a stable data format (it may
       change at any time). Only included since it *may* contain additional data
       that could be useful for developers of analysis tools.</sub>
 
 All files are written to the same directory (`activities/` by default).  Each
 activity file is prefixed by its upload timestamp and its activity id.
 
-
 `garminexport` also contains a few smaller utility programs:
 
 - `garmin-get-activity`: download a single Garmin Connect activity. Run with
   `--help`for more details.
 - `garmin-upload-activity`: uplad a single Garmin Connect activity file (`.fit`,
   `.gpx`, or `.tcx`). Run with `--help`for more details.
 
-
 ## As a library
 
 To build your own tools around the Garmin Connect API you can import the
 `garminclient` module. It handles authentication to establish a secure session
 with Garmin Connect. For example use, have a look at the command-line tools
 under [garminexport/cli](garminexport/cli).
 
+For example, in your `setup.py`, `setup.cfg`, `pyproject.toml` ([PEP
+631](https://peps.python.org/pep-0631/)) add something like:
+
+``` python
+install_requires=[
+    'garminexport',
+    # also installs 'cloudscraper' as a dependency
+    # 'garminexport[cloudflare]',
+    ...
+]
+```
+
+Note: if you happen to have
+[cloudscraper](https://github.com/VeNoMouS/cloudscraper) on your `PACKAGEPATH`
+`GarminClient` will make use of it whenever it needs to make an HTTP request.
 
 # Contribute
 
 To work on the code base you need (besides the basic prerequisites outlined
 above) to have [pipenv](https://github.com/pypa/pipenv) installed.  Create a
 `virtualenv` (an isolated development environment) and install the required
 dependencies like so:
```

### Comparing `garminexport-0.4.0/garminexport/backup.py` & `garminexport-0.4.1/garminexport/backup.py`

 * *Files identical despite different names*

### Comparing `garminexport-0.4.0/garminexport/cli/backup.py` & `garminexport-0.4.1/garminexport/cli/backup.py`

 * *Files identical despite different names*

### Comparing `garminexport-0.4.0/garminexport/cli/get_activity.py` & `garminexport-0.4.1/garminexport/cli/get_activity.py`

 * *Files identical despite different names*

### Comparing `garminexport-0.4.0/garminexport/cli/upload_activity.py` & `garminexport-0.4.1/garminexport/cli/upload_activity.py`

 * *Files identical despite different names*

### Comparing `garminexport-0.4.0/garminexport/garminclient.py` & `garminexport-0.4.1/garminexport/garminclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,27 @@
 from datetime import timedelta, datetime
 from builtins import range
 from functools import wraps
 from io import BytesIO
 
 import dateutil
 import dateutil.parser
+
+#
+# By default we use the requests library to create http clients. If built with
+# the 'cloudflare' extra, we use cloudscraper to circumvent CloudFlare's
+# anti-bot protection pages.
+#
 import requests
+session_factory = requests.session
+try:
+    import cloudscraper
+    session_factory = cloudscraper.create_scraper
+except (ImportError):
+    pass
 
 from garminexport.retryer import Retryer, ExponentialBackoffDelayStrategy, MaxRetriesStopStrategy
 
 #
 # Note: For more detailed information about the API services
 # used by this module, log in to your Garmin Connect account
 # through the web browser and visit the API documentation page
@@ -106,15 +118,16 @@
         self.connect()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.disconnect()
 
     def connect(self):
-        self.session = requests.Session()
+        log.debug("using session factory: %s", session_factory.__module__)
+        self.session = session_factory()
         self._authenticate()
 
     def disconnect(self):
         if self.session:
             self.session.close()
             self.session = None
 
@@ -226,15 +239,15 @@
         Should the index be out of bounds or the account empty, an empty list is returned.
 
         :param start_index: The index of the first activity to retrieve.
         :type start_index: int
         :param max_limit: The (maximum) number of activities to retrieve.
         :type max_limit: int
 
-        :returns: A list of activity identifiers (along with their starting timestamps).
+        :returns: A list of activity JSON dicts describing the activity
         :rtype: tuples of (int, datetime)
         """
         log.debug("fetching activities %d through %d ...", start_index, start_index + max_limit - 1)
         response = self.session.get(
             "https://connect.garmin.com/proxy/activitylist-service/activities/search/activities",
             params={"start": start_index, "limit": max_limit})
         if response.status_code != 200:
```

### Comparing `garminexport-0.4.0/garminexport/incremental_backup.py` & `garminexport-0.4.1/garminexport/incremental_backup.py`

 * *Files identical despite different names*

### Comparing `garminexport-0.4.0/garminexport/retryer.py` & `garminexport-0.4.1/garminexport/retryer.py`

 * *Files identical despite different names*

### Comparing `garminexport-0.4.0/garminexport.egg-info/PKG-INFO` & `garminexport-0.4.1/garminexport.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,140 +1,17 @@
 Metadata-Version: 2.1
 Name: garminexport
-Version: 0.4.0
+Version: 0.4.1
 Summary: Garmin Connect activity exporter and backup tool
 Home-page: https://github.com/petergardfjall/garminexport
 Author: Peter Gardfjäll
 Author-email: peter.gardfjall.work@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/petergardfjall/garminexport.git
 Project-URL: Tracker, https://github.com/petergardfjall/garminexport/issues
-Description: [![Build Status](https://travis-ci.org/petergardfjall/garminexport.svg?branch=master)](https://travis-ci.org/petergardfjall/garminexport)
-        [![PyPi release](https://img.shields.io/pypi/v/garminexport.svg)](https://img.shields.io/pypi/v/garminexport.svg)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/garminexport)
-        ![PyPI - License](https://img.shields.io/pypi/l/garminexport)
-        
-        # About
-        `garminexport` is both a library and a utility script for downloading/backing up
-        [Garmin Connect](http://connect.garmin.com/) activities to a local disk.
-        
-        The main utility script is called `garmin-backup` and performs incremental
-        backups of your Garmin account to a local directory. The first time
-        `garmin-backup` is run, it will download *all* activities. After that, it will
-        do incremental backups of your account. That is, the script will only download
-        activities that haven't already been downloaded to the backup directory.
-        
-        
-        # Installation
-        `garminexport` is available on [PyPi](https://pypi.org/) and can be installed
-        with [pip](http://pip.readthedocs.org):
-        
-            pip install garminexport
-        
-        It requires Python 3.5+.
-        
-        
-        # Usage
-        
-        
-        ## Prerequisites
-        To be of any use you need to register an account at [Garmin
-        Connect](http://connect.garmin.com/) and populate it with some activities.
-        
-        
-        ## As a command-line tool (garmin-backup)
-        
-        The backup program is run as follows (use the `--help` flag for a full list of
-        available options):
-        
-            garmin-backup --backup-dir=activities <username or email>
-        
-        Once started, the program will prompt you for your account password and then log
-        in to your Garmin Connect account to download activities to the specified backup
-        directory on your machine. The program will only download activities that aren't
-        already in the backup directory.
-        
-        Activities can be exported in any of the formats outlined below. Note that
-        by default, the program downloads all formats for every activity. Use the
-        `--format` option to narrow the selection.
-        
-        Supported export formats:
-        
-        
-          -   `gpx`: activity GPX file (XML).
-        
-              <sub>[GPX](https://en.wikipedia.org/wiki/GPS_Exchange_Format) is an open
-              format, mainly for storing GPS routes/tracks. It does support extensions
-              and Garmin appears to annotate the GPS data with, for example, heart-rate
-              and cadence, when available on your device.</sub>
-        
-          -   `tcx`: an activity TCX file (XML).
-              *Note: a `.tcx` file may not always be possible to export, for example
-              if an activity was uploaded in gpx format. In that case, Garmin won't try
-              to synthesize a tcx file.*
-        
-              <sub>[TCX](https://en.wikipedia.org/wiki/Training_Center_XML) (Training
-              Center XML) is Garmin's own XML format. It is, essentially, an extension
-              of GPX which includes more metrics and divides the GPS track into "laps"
-              as recorded by your device (with "lap summaries" for each metric).</sub>
-        
-          -   `fit`: activity FIT file (binary format).
-              *Note: a `.fit` file may not always be possible to export, for example
-              if an activity was entered manually rather than imported from a Garmin device.*
-        
-              <sub>The [FIT](https://www.thisisant.com/resources/fit/) format is the
-              "raw data type" stored in your Garmin device and should contain all
-              metrics your device is capable of tracking (GPS, heart rate, cadence,
-              etc). It's a binary format, so tools are needed to read its content.</sub>
-        
-          -   `json_summary`: activity summary file (JSON).
-        
-              <sub>Provides summary data for an activity. Seems to lack a formal schema
-              and should not be counted on as a stable data format (it may change at any
-              time). Only included since it *may* contain additional data that could be
-              useful for developers of analysis tools.</sub>
-        
-          -   `json_details`: activity details file (JSON).
-        
-              <sub>Provides detailed activity data in a JSON format. Seems to lack a
-              formal schema and should not be counted on as a stable data format (it may
-              change at any time). Only included since it *may* contain additional data
-              that could be useful for developers of analysis tools.</sub>
-        
-        All files are written to the same directory (`activities/` by default).  Each
-        activity file is prefixed by its upload timestamp and its activity id.
-        
-        
-        `garminexport` also contains a few smaller utility programs:
-        
-        - `garmin-get-activity`: download a single Garmin Connect activity. Run with
-          `--help`for more details.
-        - `garmin-upload-activity`: uplad a single Garmin Connect activity file (`.fit`,
-          `.gpx`, or `.tcx`). Run with `--help`for more details.
-        
-        
-        ## As a library
-        
-        To build your own tools around the Garmin Connect API you can import the
-        `garminclient` module. It handles authentication to establish a secure session
-        with Garmin Connect. For example use, have a look at the command-line tools
-        under [garminexport/cli](garminexport/cli).
-        
-        
-        # Contribute
-        
-        To work on the code base you need (besides the basic prerequisites outlined
-        above) to have [pipenv](https://github.com/pypa/pipenv) installed.  Create a
-        `virtualenv` (an isolated development environment) and install the required
-        dependencies like so:
-        
-        
-            make venv
-            # or similarly: pipenv install
-        
 Keywords: garmin export backup
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -142,7 +19,161 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5.*, <4
 Description-Content-Type: text/markdown
+Provides-Extra: cloudflare
+License-File: LICENSE
+
+[![Build Status](https://travis-ci.org/petergardfjall/garminexport.svg?branch=master)](https://travis-ci.org/petergardfjall/garminexport)
+[![PyPi release](https://img.shields.io/pypi/v/garminexport.svg)](https://img.shields.io/pypi/v/garminexport.svg)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/garminexport)
+![PyPI - License](https://img.shields.io/pypi/l/garminexport)
+
+# About
+
+`garminexport` is both a library and a tool for downloading/backing up [Garmin
+Connect](http://connect.garmin.com/) activities to a local disk.
+
+The main utility script is called `garmin-backup` and performs incremental
+backups of your Garmin account to a local directory. The first time
+`garmin-backup` is run, it will download *all* activities. After that, it will
+do incremental backups of your account. That is, the script will only download
+activities that haven't already been downloaded to the backup directory.
+
+
+# Installation
+
+`garminexport` is available on [PyPi](https://pypi.org/) and can be installed
+with [pip](http://pip.readthedocs.org):
+
+``` bash
+pip install garminexport
+```
+
+To install `garminexport` with support to circumvent Cloudflare's bot protection
+(which has been known to impact some users) you can install the module with the
+`cloudflare`
+[extra](https://setuptools.pypa.io/en/latest/userguide/dependency_management.html#optional-dependencies) like so:
+
+``` bash
+pip install garminexport[cloudflare]
+```
+
+This replaces the default [requests](https://github.com/psf/requests) library
+with [cloudscraper](https://github.com/VeNoMouS/cloudscraper) for HTTP request.
+
+# Usage
+
+## Prerequisites
+To be of any use you need to register an account at [Garmin
+Connect](http://connect.garmin.com/) and populate it with some activities.
+
+
+## As a command-line tool (garmin-backup)
+
+The backup program is run as follows (use the `--help` flag for a full list of
+available options):
+
+``` bash
+garmin-backup --backup-dir=activities <username or email>
+```
+
+Once started, the program will prompt you for your account password and then log
+in to your Garmin Connect account to download activities to the specified backup
+directory on your machine. The program will only download activities that aren't
+already in the backup directory.
+
+Activities can be exported in any of the formats outlined below. Note that
+by default, the program downloads all formats for every activity. Use the
+`--format` option to narrow the selection.
+
+Supported export formats:
+
+
+  -   `gpx`: activity GPX file (XML).
+
+      <sub>[GPX](https://en.wikipedia.org/wiki/GPS_Exchange_Format) is an open
+      format, mainly for storing GPS routes/tracks. It does support extensions
+      and Garmin appears to annotate the GPS data with, for example, heart-rate
+      and cadence, when available on your device.</sub>
+
+  -   `tcx`: an activity TCX file (XML).
+      *Note: a `.tcx` file may not always be possible to export, for example
+      if an activity was uploaded in gpx format. In that case, Garmin won't try
+      to synthesize a tcx file.*
+
+      <sub>[TCX](https://en.wikipedia.org/wiki/Training_Center_XML) (Training
+      Center XML) is Garmin's own XML format. It is, essentially, an extension
+      of GPX which includes more metrics and divides the GPS track into "laps"
+      as recorded by your device (with "lap summaries" for each metric).</sub>
+
+  -   `fit`: activity FIT file (binary format).
+      *Note: a `.fit` file may not always be possible to export, for example
+      if an activity was entered manually rather than imported from a Garmin device.*
+
+      <sub>The [FIT](https://www.thisisant.com/resources/fit/) format is the
+      "raw data type" stored in your Garmin device and should contain all
+      metrics your device is capable of tracking (GPS, heart rate, cadence,
+      etc). It's a binary format, so tools are needed to read its content.</sub>
+
+  -   `json_summary`: activity summary file (JSON).
+
+      <sub>Provides summary data for an activity. Seems to lack a formal schema
+      and should not be counted on as a stable data format (it may change at any
+      time). Only included since it *may* contain additional data that could be
+      useful for developers of analysis tools.</sub>
+
+  -   `json_details`: activity details file (JSON).
+
+      <sub>Provides detailed activity data in a JSON format. Seems to lack a
+      formal schema and should not be counted on as a stable data format (it may
+      change at any time). Only included since it *may* contain additional data
+      that could be useful for developers of analysis tools.</sub>
+
+All files are written to the same directory (`activities/` by default).  Each
+activity file is prefixed by its upload timestamp and its activity id.
+
+`garminexport` also contains a few smaller utility programs:
+
+- `garmin-get-activity`: download a single Garmin Connect activity. Run with
+  `--help`for more details.
+- `garmin-upload-activity`: uplad a single Garmin Connect activity file (`.fit`,
+  `.gpx`, or `.tcx`). Run with `--help`for more details.
+
+## As a library
+
+To build your own tools around the Garmin Connect API you can import the
+`garminclient` module. It handles authentication to establish a secure session
+with Garmin Connect. For example use, have a look at the command-line tools
+under [garminexport/cli](garminexport/cli).
+
+For example, in your `setup.py`, `setup.cfg`, `pyproject.toml` ([PEP
+631](https://peps.python.org/pep-0631/)) add something like:
+
+``` python
+install_requires=[
+    'garminexport',
+    # also installs 'cloudscraper' as a dependency
+    # 'garminexport[cloudflare]',
+    ...
+]
+```
+
+Note: if you happen to have
+[cloudscraper](https://github.com/VeNoMouS/cloudscraper) on your `PACKAGEPATH`
+`GarminClient` will make use of it whenever it needs to make an HTTP request.
+
+# Contribute
+
+To work on the code base you need (besides the basic prerequisites outlined
+above) to have [pipenv](https://github.com/pypa/pipenv) installed.  Create a
+`virtualenv` (an isolated development environment) and install the required
+dependencies like so:
+
+
+    make venv
+    # or similarly: pipenv install
+
+
```

### Comparing `garminexport-0.4.0/garminexport.egg-info/SOURCES.txt` & `garminexport-0.4.1/garminexport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garminexport-0.4.0/setup.py` & `garminexport-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,26 @@
     long_description = f.read()
 
 requires = [
     'requests>=2.0,<3',
     'python-dateutil~=2.4',
 ]
 
+extras_require = {
+    'cloudflare': ['cloudscraper~=1.2'],
+}
+
 test_requires = [
     'nose~=1.3',
     'coverage~=4.2',
     'mock~=2.0',
 ]
 
 setup(name='garminexport',
-      version='0.4.0',
+      version='0.4.1',
       description='Garmin Connect activity exporter and backup tool',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Peter Gardfjäll',
       author_email='peter.gardfjall.work@gmail.com',
 
       classifiers=[
@@ -55,14 +59,15 @@
       packages=[
           'garminexport',
           'garminexport.cli',
       ],
 
       python_requires='>=3.5.*, <4',
       install_requires=requires,
+      extras_require=extras_require,
       test_requires=test_requires,
       entry_points={
         'console_scripts': [
             'garmin-backup = garminexport.cli.backup:main',
             'garmin-get-activity = garminexport.cli.get_activity:main',
             'garmin-upload-activity = garminexport.cli.upload_activity:main',
         ],
```

