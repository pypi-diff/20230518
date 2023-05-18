# Comparing `tmp/race_report_by_ng-1.0.0.tar.gz` & `tmp/race_report_by_ng-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "race_report_by_ng-1.0.0.tar", max compression
+gzip compressed data, was "race_report_by_ng-1.0.1.tar", max compression
```

## Comparing `race_report_by_ng-1.0.0.tar` & `race_report_by_ng-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rwxr-xr-x   0        0        0     1073 2023-05-17 09:11:19.161292 race_report_by_ng-1.0.0/LICENSE
--rwxr-xr-x   0        0        0     5718 2023-05-18 08:39:20.682565 race_report_by_ng-1.0.0/README.md
--rwxr-xr-x   0        0        0      475 2023-05-18 14:44:38.670117 race_report_by_ng-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0      155 2023-05-18 09:00:22.023185 race_report_by_ng-1.0.0/race_report_by_ng/__init__.py
--rwxr-xr-x   0        0        0     8379 2023-05-18 14:43:01.098685 race_report_by_ng-1.0.0/race_report_by_ng/report.py
--rwxr-xr-x   0        0        0     2271 2023-05-18 14:45:48.519668 race_report_by_ng-1.0.0/race_report_by_ng/report_cli.py
--rw-r--r--   0        0        0     6355 1970-01-01 00:00:00.000000 race_report_by_ng-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-17 09:11:19.161292 race_report_by_ng-1.0.1/LICENSE
+-rwxr-xr-x   0        0        0     5718 2023-05-18 08:39:20.682565 race_report_by_ng-1.0.1/README.md
+-rwxr-xr-x   0        0        0      475 2023-05-18 15:03:24.735005 race_report_by_ng-1.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0      155 2023-05-18 09:00:22.023185 race_report_by_ng-1.0.1/race_report_by_ng/__init__.py
+-rwxr-xr-x   0        0        0      579 2023-05-18 15:02:37.408352 race_report_by_ng-1.0.1/race_report_by_ng/logger/logger.py
+-rwxr-xr-x   0        0        0     2103 2023-05-18 15:02:43.279231 race_report_by_ng-1.0.1/race_report_by_ng/logger/report.log
+-rwxr-xr-x   0        0        0     8397 2023-05-18 15:03:07.354188 race_report_by_ng-1.0.1/race_report_by_ng/report.py
+-rwxr-xr-x   0        0        0     2271 2023-05-18 14:45:48.519668 race_report_by_ng-1.0.1/race_report_by_ng/report_cli.py
+-rw-r--r--   0        0        0     6355 1970-01-01 00:00:00.000000 race_report_by_ng-1.0.1/PKG-INFO
```

### Comparing `race_report_by_ng-1.0.0/LICENSE` & `race_report_by_ng-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `race_report_by_ng-1.0.0/README.md` & `race_report_by_ng-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `race_report_by_ng-1.0.0/race_report_by_ng/report.py` & `race_report_by_ng-1.0.1/race_report_by_ng/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime, timedelta
 
 from prettytable import PrettyTable
 from termcolor import colored
 
-from logger.logger import report_logger
+from race_report_by_ng.logger.logger import report_logger
 
 
 TABLE_FIELD_NAMES = ["Place", "Driver name", "Team", "Best lap"]
 TIME_FORMAT = "%Y-%m-%d_%H:%M:%S.%f"
 NUMBER_TOP_DRIVERS = 15  # The number of drivers who will be in the TOP table
```

### Comparing `race_report_by_ng-1.0.0/race_report_by_ng/report_cli.py` & `race_report_by_ng-1.0.1/race_report_by_ng/report_cli.py`

 * *Files identical despite different names*

### Comparing `race_report_by_ng-1.0.0/PKG-INFO` & `race_report_by_ng-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: race-report-by-ng
-Version: 1.0.0
+Version: 1.0.1
 Summary: Application that reads data from 3 files, orders racers by time, and prints a report showing two tables: the top 15 racers and the remaining racers.
 License: MIT
 Author: Nazar Hots
 Author-email: gotsjob@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

