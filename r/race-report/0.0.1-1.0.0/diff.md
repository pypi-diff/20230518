# Comparing `tmp/race_report-0.0.1.tar.gz` & `tmp/race_report-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "race_report-0.0.1.tar", max compression
+gzip compressed data, was "race_report-1.0.0.tar", max compression
```

## Comparing `race_report-0.0.1.tar` & `race_report-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1073 2023-05-17 09:11:19.161292 race_report-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     5718 2023-05-18 08:39:20.682565 race_report-0.0.1/README.md
--rwxr-xr-x   0        0        0      469 2023-05-18 15:15:07.232360 race_report-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      155 2023-05-18 15:11:23.820078 race_report-0.0.1/race_report/__init__.py
--rwxr-xr-x   0        0        0     7753 2023-05-18 15:14:47.963979 race_report-0.0.1/race_report/report.py
--rwxr-xr-x   0        0        0     2132 2023-05-18 15:14:26.076512 race_report-0.0.1/race_report/report_cli.py
--rw-r--r--   0        0        0     6349 1970-01-01 00:00:00.000000 race_report-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-17 09:11:19.161292 race_report-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0     5712 2023-05-18 15:19:33.481233 race_report-1.0.0/README.md
+-rwxr-xr-x   0        0        0      469 2023-05-18 15:18:19.652661 race_report-1.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0      155 2023-05-18 15:11:23.820078 race_report-1.0.0/race_report/__init__.py
+-rwxr-xr-x   0        0        0     7753 2023-05-18 15:14:47.963979 race_report-1.0.0/race_report/report.py
+-rwxr-xr-x   0        0        0     2132 2023-05-18 15:14:26.076512 race_report-1.0.0/race_report/report_cli.py
+-rw-r--r--   0        0        0     6343 1970-01-01 00:00:00.000000 race_report-1.0.0/PKG-INFO
```

### Comparing `race_report-0.0.1/LICENSE` & `race_report-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `race_report-0.0.1/README.md` & `race_report-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Installation
 Clone this repository to your local machine:
 
 
 Use the manager [pip](https://pip.pypa.io/en/stable/) to install package:
 
 ```bash
-pip install race_report_by_ng
+pip install race-report
 ```
 
 ## Summary
 Application that read data from **3 files**, order racers by time and print report that shows 2 tables: the top 15 racers and other racers.
 🔴 **Data should include 3 files: "start.log", "end.log", abbreviations.txt.** 🔴
 
 The files **"start.log"** and **"end.log"** should have lines in the format **"SVF2018-05-24_12:02:58.917"**, where:
```

### Comparing `race_report-0.0.1/race_report/report.py` & `race_report-1.0.0/race_report/report.py`

 * *Files identical despite different names*

### Comparing `race_report-0.0.1/race_report/report_cli.py` & `race_report-1.0.0/race_report/report_cli.py`

 * *Files identical despite different names*

### Comparing `race_report-0.0.1/PKG-INFO` & `race_report-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: race-report
-Version: 0.0.1
+Version: 1.0.0
 Summary: Application that reads data from 3 files, orders racers by time, and prints a report showing two tables: the top 15 racers and the remaining racers.
 License: MIT
 Author: Nazar Hots
 Author-email: gotsjob@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 ## Installation
 Clone this repository to your local machine:
 
 
 Use the manager [pip](https://pip.pypa.io/en/stable/) to install package:
 
 ```bash
-pip install race_report_by_ng
+pip install race-report
 ```
 
 ## Summary
 Application that read data from **3 files**, order racers by time and print report that shows 2 tables: the top 15 racers and other racers.
 🔴 **Data should include 3 files: "start.log", "end.log", abbreviations.txt.** 🔴
 
 The files **"start.log"** and **"end.log"** should have lines in the format **"SVF2018-05-24_12:02:58.917"**, where:
```

