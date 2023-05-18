# Comparing `tmp/python-cli-scheduler-1.0.0.tar.gz` & `tmp/python-cli-scheduler-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cli-scheduler-1.0.0.tar", last modified: Fri May 12 08:30:37 2023, max compression
+gzip compressed data, was "python-cli-scheduler-1.1.0.tar", last modified: Thu May 18 05:06:59 2023, max compression
```

## Comparing `python-cli-scheduler-1.0.0.tar` & `python-cli-scheduler-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 08:30:37.866618 python-cli-scheduler-1.0.0/
--rw-r--r--   0 lam        (502) staff       (20)     1129 2022-11-08 09:34:27.000000 python-cli-scheduler-1.0.0/LICENSE
--rw-r--r--   0 lam        (502) staff       (20)     2273 2023-05-12 08:30:37.865832 python-cli-scheduler-1.0.0/PKG-INFO
--rw-r--r--   0 lam        (502) staff       (20)     1708 2023-05-12 06:43:02.000000 python-cli-scheduler-1.0.0/README.md
--rw-r--r--   0 lam        (502) staff       (20)       89 2022-11-08 09:34:27.000000 python-cli-scheduler-1.0.0/pyproject.toml
--rw-r--r--   0 lam        (502) staff       (20)       38 2023-05-12 08:30:37.866833 python-cli-scheduler-1.0.0/setup.cfg
--rw-r--r--   0 lam        (502) staff       (20)     1029 2023-05-12 08:19:55.000000 python-cli-scheduler-1.0.0/setup.py
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 08:30:37.836163 python-cli-scheduler-1.0.0/src/
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 08:30:37.847374 python-cli-scheduler-1.0.0/src/cli_scheduler/
--rw-r--r--   0 lam        (502) staff       (20)       22 2023-05-12 08:30:01.000000 python-cli-scheduler-1.0.0/src/cli_scheduler/__init__.py
--rw-r--r--   0 lam        (502) staff       (20)     2428 2023-05-12 04:29:26.000000 python-cli-scheduler-1.0.0/src/cli_scheduler/cli_job.py
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 08:30:37.849960 python-cli-scheduler-1.0.0/src/cli_scheduler/constants/
--rw-r--r--   0 lam        (502) staff       (20)        0 2022-11-08 09:41:36.000000 python-cli-scheduler-1.0.0/src/cli_scheduler/constants/__init__.py
--rw-r--r--   0 lam        (502) staff       (20)      338 2023-05-12 04:29:26.000000 python-cli-scheduler-1.0.0/src/cli_scheduler/constants/time_constants.py
--rw-r--r--   0 lam        (502) staff       (20)     1874 2022-11-09 03:16:02.000000 python-cli-scheduler-1.0.0/src/cli_scheduler/handler.py
--rw-r--r--   0 lam        (502) staff       (20)     5350 2023-05-12 04:29:26.000000 python-cli-scheduler-1.0.0/src/cli_scheduler/scheduler_job.py
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 08:30:37.858194 python-cli-scheduler-1.0.0/src/cli_scheduler/utils/
--rw-r--r--   0 lam        (502) staff       (20)        0 2022-11-08 09:32:37.000000 python-cli-scheduler-1.0.0/src/cli_scheduler/utils/__init__.py
--rw-r--r--   0 lam        (502) staff       (20)      512 2022-11-08 09:34:27.000000 python-cli-scheduler-1.0.0/src/cli_scheduler/utils/function_utils.py
--rw-r--r--   0 lam        (502) staff       (20)      777 2022-10-18 03:30:15.000000 python-cli-scheduler-1.0.0/src/cli_scheduler/utils/logger_utils.py
--rw-r--r--   0 lam        (502) staff       (20)      464 2023-05-12 05:00:35.000000 python-cli-scheduler-1.0.0/src/cli_scheduler/utils/time_utils.py
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 08:30:37.864817 python-cli-scheduler-1.0.0/src/python_cli_scheduler.egg-info/
--rw-r--r--   0 lam        (502) staff       (20)     2273 2023-05-12 08:30:37.000000 python-cli-scheduler-1.0.0/src/python_cli_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 lam        (502) staff       (20)      598 2023-05-12 08:30:37.000000 python-cli-scheduler-1.0.0/src/python_cli_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 lam        (502) staff       (20)        1 2023-05-12 08:30:37.000000 python-cli-scheduler-1.0.0/src/python_cli_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 lam        (502) staff       (20)       14 2023-05-12 08:30:37.000000 python-cli-scheduler-1.0.0/src/python_cli_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-18 05:06:59.433167 python-cli-scheduler-1.1.0/
+-rw-r--r--   0 lam        (502) staff       (20)     1129 2022-11-08 09:34:27.000000 python-cli-scheduler-1.1.0/LICENSE
+-rw-r--r--   0 lam        (502) staff       (20)     2273 2023-05-18 05:06:59.432618 python-cli-scheduler-1.1.0/PKG-INFO
+-rw-r--r--   0 lam        (502) staff       (20)     1708 2023-05-12 06:43:02.000000 python-cli-scheduler-1.1.0/README.md
+-rw-r--r--   0 lam        (502) staff       (20)       89 2022-11-08 09:34:27.000000 python-cli-scheduler-1.1.0/pyproject.toml
+-rw-r--r--   0 lam        (502) staff       (20)       38 2023-05-18 05:06:59.433376 python-cli-scheduler-1.1.0/setup.cfg
+-rw-r--r--   0 lam        (502) staff       (20)     1058 2023-05-18 04:52:27.000000 python-cli-scheduler-1.1.0/setup.py
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-18 05:06:59.416403 python-cli-scheduler-1.1.0/src/
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-18 05:06:59.421587 python-cli-scheduler-1.1.0/src/cli_scheduler/
+-rw-r--r--   0 lam        (502) staff       (20)       22 2023-05-18 05:06:41.000000 python-cli-scheduler-1.1.0/src/cli_scheduler/__init__.py
+-rw-r--r--   0 lam        (502) staff       (20)     2428 2023-05-12 04:29:26.000000 python-cli-scheduler-1.1.0/src/cli_scheduler/cli_job.py
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-18 05:06:59.422585 python-cli-scheduler-1.1.0/src/cli_scheduler/constants/
+-rw-r--r--   0 lam        (502) staff       (20)        0 2022-11-08 09:41:36.000000 python-cli-scheduler-1.1.0/src/cli_scheduler/constants/__init__.py
+-rw-r--r--   0 lam        (502) staff       (20)      338 2023-05-12 04:29:26.000000 python-cli-scheduler-1.1.0/src/cli_scheduler/constants/time_constants.py
+-rw-r--r--   0 lam        (502) staff       (20)     1874 2022-11-09 03:16:02.000000 python-cli-scheduler-1.1.0/src/cli_scheduler/handler.py
+-rw-r--r--   0 lam        (502) staff       (20)     5494 2023-05-18 04:34:28.000000 python-cli-scheduler-1.1.0/src/cli_scheduler/scheduler_job.py
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-18 05:06:59.426109 python-cli-scheduler-1.1.0/src/cli_scheduler/utils/
+-rw-r--r--   0 lam        (502) staff       (20)        0 2022-11-08 09:32:37.000000 python-cli-scheduler-1.1.0/src/cli_scheduler/utils/__init__.py
+-rw-r--r--   0 lam        (502) staff       (20)      512 2022-11-08 09:34:27.000000 python-cli-scheduler-1.1.0/src/cli_scheduler/utils/function_utils.py
+-rw-r--r--   0 lam        (502) staff       (20)      777 2022-10-18 03:30:15.000000 python-cli-scheduler-1.1.0/src/cli_scheduler/utils/logger_utils.py
+-rw-r--r--   0 lam        (502) staff       (20)      464 2023-05-12 05:00:35.000000 python-cli-scheduler-1.1.0/src/cli_scheduler/utils/time_utils.py
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-18 05:06:59.430183 python-cli-scheduler-1.1.0/src/python_cli_scheduler.egg-info/
+-rw-r--r--   0 lam        (502) staff       (20)     2273 2023-05-18 05:06:59.000000 python-cli-scheduler-1.1.0/src/python_cli_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 lam        (502) staff       (20)      673 2023-05-18 05:06:59.000000 python-cli-scheduler-1.1.0/src/python_cli_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 lam        (502) staff       (20)        1 2023-05-18 05:06:59.000000 python-cli-scheduler-1.1.0/src/python_cli_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 lam        (502) staff       (20)       14 2023-05-18 05:06:59.000000 python-cli-scheduler-1.1.0/src/python_cli_scheduler.egg-info/requires.txt
+-rw-r--r--   0 lam        (502) staff       (20)       14 2023-05-18 05:06:59.000000 python-cli-scheduler-1.1.0/src/python_cli_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-18 05:06:59.430904 python-cli-scheduler-1.1.0/tests/
+-rw-r--r--   0 lam        (502) staff       (20)      322 2023-05-18 04:51:21.000000 python-cli-scheduler-1.1.0/tests/test_scheduler_job.py
```

### Comparing `python-cli-scheduler-1.0.0/LICENSE` & `python-cli-scheduler-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-cli-scheduler-1.0.0/PKG-INFO` & `python-cli-scheduler-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cli-scheduler
-Version: 1.0.0
+Version: 1.1.0
 Summary: Support scheduling of task via command line interface.
 Home-page: https://github.com/hoangthanhlamm/python-cli-scheduler
 Author: Lam Hoang
 Author-email: hoangthanhlamm@gmail.com
 Project-URL: Bug Tracker, https://github.com/hoangthanhlamm/python-cli-scheduler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-cli-scheduler-1.0.0/README.md` & `python-cli-scheduler-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python-cli-scheduler-1.0.0/setup.py` & `python-cli-scheduler-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,9 +22,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
-    install_requires=[],
+    install_requires=[
+        "pytest==7.3.1"
+    ],
 )
```

### Comparing `python-cli-scheduler-1.0.0/src/cli_scheduler/cli_job.py` & `python-cli-scheduler-1.1.0/src/cli_scheduler/cli_job.py`

 * *Files identical despite different names*

### Comparing `python-cli-scheduler-1.0.0/src/cli_scheduler/handler.py` & `python-cli-scheduler-1.1.0/src/cli_scheduler/handler.py`

 * *Files identical despite different names*

### Comparing `python-cli-scheduler-1.0.0/src/cli_scheduler/scheduler_job.py` & `python-cli-scheduler-1.1.0/src/cli_scheduler/scheduler_job.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,48 +60,50 @@
 
         self.interval = kwargs.get('interval')
         self.end_timestamp = kwargs.get('end_timestamp')
         self.retry = kwargs.get('retry', True)
         self.delay = kwargs.get('delay', 0)
         self.run_now = kwargs.get('run_now', True)
 
+        if (not self.run_now) and (self.interval is None):
+            raise ValueError('At least one of the two parameters <run_now> and <interval> must be set positive value')
+
         self.next_synced_timestamp = None
 
         self.logger = get_logger(self.__class__.__name__)
 
     def run(self, *args, **kwargs):
         self._pre_start()
-        counter = 0
         while True:
             # Check run now. If not, wait to the first execute
             if not self.run_now:
                 self._get_next_synced_timestamp()
-                if self._check_finish(counter):
+                if self._check_finish():
                     break
                 self._wait_to_next_synced()
 
             try:
                 self._start()
                 self._execute(*args, **kwargs)
             except Exception as ex:
                 self._handle_exception(ex)
                 if self.retry:
                     self._retry()
                     self.run_now = True  # To retry now
                     continue
 
-            counter += 1
             self.run_now = False  # To wait for the next execute
             self._end()
 
         self._follow_end()
 
     def _get_next_synced_timestamp(self):
-        self.next_synced_timestamp = round_timestamp(
-            self.next_synced_timestamp or int(time.time()), round_time=self.interval) + self.interval + self.delay
+        if self.interval is not None:
+            self.next_synced_timestamp = round_timestamp(
+                self.next_synced_timestamp or int(time.time()), round_time=self.interval) + self.interval + self.delay
 
         # Get the next execute timestamp
         return self.next_synced_timestamp
 
     def _wait_to_next_synced(self):
         # Sleep to next execute time
         time_sleep = self.next_synced_timestamp - time.time()
@@ -109,17 +111,17 @@
             self.logger.info(f'Waiting {round(time_sleep, 3)} seconds to the next execute [{human_readable_time(self.next_synced_timestamp)}]')
             time.sleep(time_sleep)
 
     def _handle_exception(self, ex):
         self.logger.exception(ex)
         self.logger.warning('Something went wrong!!!')
 
-    def _check_finish(self, counter):
+    def _check_finish(self):
         # Check if not repeat
-        if (self.interval is None) and (not counter):
+        if self.interval is None:
             return True
 
         # Check if over end timestamp
         if (self.end_timestamp is not None) and (self.next_synced_timestamp > self.end_timestamp):
             return True
 
         return False
```

### Comparing `python-cli-scheduler-1.0.0/src/cli_scheduler/utils/function_utils.py` & `python-cli-scheduler-1.1.0/src/cli_scheduler/utils/function_utils.py`

 * *Files identical despite different names*

### Comparing `python-cli-scheduler-1.0.0/src/cli_scheduler/utils/logger_utils.py` & `python-cli-scheduler-1.1.0/src/cli_scheduler/utils/logger_utils.py`

 * *Files identical despite different names*

### Comparing `python-cli-scheduler-1.0.0/src/python_cli_scheduler.egg-info/PKG-INFO` & `python-cli-scheduler-1.1.0/src/python_cli_scheduler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cli-scheduler
-Version: 1.0.0
+Version: 1.1.0
 Summary: Support scheduling of task via command line interface.
 Home-page: https://github.com/hoangthanhlamm/python-cli-scheduler
 Author: Lam Hoang
 Author-email: hoangthanhlamm@gmail.com
 Project-URL: Bug Tracker, https://github.com/hoangthanhlamm/python-cli-scheduler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

