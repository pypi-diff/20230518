# Comparing `tmp/simpervisor-0.4.tar.gz` & `tmp/simpervisor-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simpervisor-0.4.tar", last modified: Tue Jan  5 05:42:33 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `simpervisor-0.4.tar` & `simpervisor-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 yuvipanda   (502) staff       (20)        0 2021-01-05 05:42:33.522925 simpervisor-0.4/
--rw-r--r--   0 yuvipanda   (502) staff       (20)     1510 2021-01-05 05:41:12.000000 simpervisor-0.4/LICENSE
--rw-r--r--   0 yuvipanda   (502) staff       (20)       16 2021-01-05 05:41:12.000000 simpervisor-0.4/MANIFEST.in
--rw-r--r--   0 yuvipanda   (502) staff       (20)      260 2021-01-05 05:42:33.523099 simpervisor-0.4/PKG-INFO
--rw-r--r--   0 yuvipanda   (502) staff       (20)      347 2021-01-05 05:41:12.000000 simpervisor-0.4/README.rst
--rw-r--r--   0 yuvipanda   (502) staff       (20)       52 2021-01-05 05:41:12.000000 simpervisor-0.4/pyproject.toml
--rw-r--r--   0 yuvipanda   (502) staff       (20)       74 2021-01-05 05:42:33.523988 simpervisor-0.4/setup.cfg
--rw-r--r--   0 yuvipanda   (502) staff       (20)      319 2021-01-05 05:41:32.000000 simpervisor-0.4/setup.py
-drwxr-xr-x   0 yuvipanda   (502) staff       (20)        0 2021-01-05 05:42:33.519992 simpervisor-0.4/simpervisor/
--rw-r--r--   0 yuvipanda   (502) staff       (20)       70 2021-01-05 05:41:12.000000 simpervisor-0.4/simpervisor/__init__.py
--rw-r--r--   0 yuvipanda   (502) staff       (20)      676 2021-01-05 05:41:12.000000 simpervisor-0.4/simpervisor/atexitasync.py
--rw-r--r--   0 yuvipanda   (502) staff       (20)     8994 2021-01-05 05:41:12.000000 simpervisor-0.4/simpervisor/process.py
-drwxr-xr-x   0 yuvipanda   (502) staff       (20)        0 2021-01-05 05:42:33.522483 simpervisor-0.4/simpervisor.egg-info/
--rw-r--r--   0 yuvipanda   (502) staff       (20)      260 2021-01-05 05:42:33.000000 simpervisor-0.4/simpervisor.egg-info/PKG-INFO
--rw-r--r--   0 yuvipanda   (502) staff       (20)      278 2021-01-05 05:42:33.000000 simpervisor-0.4/simpervisor.egg-info/SOURCES.txt
--rw-r--r--   0 yuvipanda   (502) staff       (20)        1 2021-01-05 05:42:33.000000 simpervisor-0.4/simpervisor.egg-info/dependency_links.txt
--rw-r--r--   0 yuvipanda   (502) staff       (20)       12 2021-01-05 05:42:33.000000 simpervisor-0.4/simpervisor.egg-info/top_level.txt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 simpervisor-1.0.0/.flake8
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 simpervisor-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 simpervisor-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 simpervisor-1.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 simpervisor-1.0.0/RELEASE.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 simpervisor-1.0.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 simpervisor-1.0.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 simpervisor-1.0.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 simpervisor-1.0.0/simpervisor/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 simpervisor-1.0.0/simpervisor/_version.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 simpervisor-1.0.0/simpervisor/atexitasync.py
+-rw-r--r--   0        0        0    12745 2020-02-02 00:00:00.000000 simpervisor-1.0.0/simpervisor/process.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 simpervisor-1.0.0/tests/test_atexitasync.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 simpervisor-1.0.0/tests/test_ready.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 simpervisor-1.0.0/tests/test_signals.py
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 simpervisor-1.0.0/tests/test_simpervisor.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 simpervisor-1.0.0/tests/child_scripts/signalprinter.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 simpervisor-1.0.0/tests/child_scripts/signalsupervisor.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 simpervisor-1.0.0/tests/child_scripts/simplehttpserver.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 simpervisor-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 simpervisor-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 simpervisor-1.0.0/README.md
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 simpervisor-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 simpervisor-1.0.0/PKG-INFO
```

### Comparing `simpervisor-0.4/LICENSE` & `simpervisor-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simpervisor-0.4/simpervisor/atexitasync.py` & `simpervisor-1.0.0/simpervisor/atexitasync.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """
 asyncio aware version of atexit.
 
 Handles SIGINT and SIGTERM, unlike atexit
 """
 import signal
-import asyncio
 import sys
 
 _handlers = []
 
 signal_handler_set = False
 
+
 def add_handler(handler):
     global signal_handler_set
     if not signal_handler_set:
-        loop = asyncio.get_event_loop()
-        loop.add_signal_handler(signal.SIGINT, _handle_signal, signal.SIGINT)
-        loop.add_signal_handler(signal.SIGTERM, _handle_signal, signal.SIGTERM)
+        signal.signal(signal.SIGINT, _handle_signal)
+        signal.signal(signal.SIGTERM, _handle_signal)
         signal_handler_set = True
     _handlers.append(handler)
 
+
 def remove_handler(handler):
     _handlers.remove(handler)
 
-def _handle_signal(signum):
+
+def _handle_signal(signum, *args):
+    # Windows doesn't support SIGINT. Replacing it with CTRL_C_EVENT so that it
+    # can used with subprocess.Popen.send_signal
+    if signum == signal.SIGINT and sys.platform == "win32":
+        signum = signal.CTRL_C_EVENT
     for handler in _handlers:
         handler(signum)
-    sys.exit(0)
+    sys.exit(0)
```

