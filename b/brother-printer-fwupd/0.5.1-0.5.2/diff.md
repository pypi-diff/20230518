# Comparing `tmp/brother_printer_fwupd-0.5.1.tar.gz` & `tmp/brother_printer_fwupd-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brother_printer_fwupd-0.5.1.tar", max compression
+gzip compressed data, was "brother_printer_fwupd-0.5.2.tar", max compression
```

## Comparing `brother_printer_fwupd-0.5.1.tar` & `brother_printer_fwupd-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35150 2019-05-05 22:45:01.929067 brother_printer_fwupd-0.5.1/LICENSE
--rw-r--r--   0        0        0       75 2022-06-04 19:12:12.377682 brother_printer_fwupd-0.5.1/brother_printer_fwupd/__init__.py
--rwxr-xr-x   0        0        0     6212 2023-05-18 13:46:41.285683 brother_printer_fwupd-0.5.1/brother_printer_fwupd/__main__.py
--rw-r--r--   0        0        0     7080 2023-05-18 13:19:45.294187 brother_printer_fwupd-0.5.1/brother_printer_fwupd/autodiscover_printer.py
--rw-r--r--   0        0        0     3128 2023-05-18 13:19:29.797478 brother_printer_fwupd-0.5.1/brother_printer_fwupd/firmware_downloader.py
--rw-r--r--   0        0        0      739 2023-05-18 11:50:56.235324 brother_printer_fwupd-0.5.1/brother_printer_fwupd/firmware_uploader.py
--rw-r--r--   0        0        0     1718 2023-05-18 11:55:02.716491 brother_printer_fwupd-0.5.1/brother_printer_fwupd/models.py
--rw-r--r--   0        0        0     3050 2022-06-04 20:30:23.818775 brother_printer_fwupd-0.5.1/brother_printer_fwupd/snmp_info.py
--rw-r--r--   0        0        0     5853 2023-05-18 13:37:45.074134 brother_printer_fwupd-0.5.1/brother_printer_fwupd/utils.py
--rw-r--r--   0        0        0      875 2023-05-18 13:47:29.349154 brother_printer_fwupd-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 brother_printer_fwupd-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35150 2019-05-05 22:45:01.929067 brother_printer_fwupd-0.5.2/LICENSE
+-rw-r--r--   0        0        0       75 2022-06-04 19:12:12.377682 brother_printer_fwupd-0.5.2/brother_printer_fwupd/__init__.py
+-rwxr-xr-x   0        0        0     6212 2023-05-18 13:46:41.285683 brother_printer_fwupd-0.5.2/brother_printer_fwupd/__main__.py
+-rw-r--r--   0        0        0     7080 2023-05-18 13:19:45.294187 brother_printer_fwupd-0.5.2/brother_printer_fwupd/autodiscover_printer.py
+-rw-r--r--   0        0        0     3128 2023-05-18 13:19:29.797478 brother_printer_fwupd-0.5.2/brother_printer_fwupd/firmware_downloader.py
+-rw-r--r--   0        0        0      739 2023-05-18 11:50:56.235324 brother_printer_fwupd-0.5.2/brother_printer_fwupd/firmware_uploader.py
+-rw-r--r--   0        0        0     1718 2023-05-18 11:55:02.716491 brother_printer_fwupd-0.5.2/brother_printer_fwupd/models.py
+-rw-r--r--   0        0        0     3050 2022-06-04 20:30:23.818775 brother_printer_fwupd-0.5.2/brother_printer_fwupd/snmp_info.py
+-rw-r--r--   0        0        0     5743 2023-05-18 13:51:46.323222 brother_printer_fwupd-0.5.2/brother_printer_fwupd/utils.py
+-rw-r--r--   0        0        0      875 2023-05-18 13:52:17.733311 brother_printer_fwupd-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 brother_printer_fwupd-0.5.2/PKG-INFO
```

### Comparing `brother_printer_fwupd-0.5.1/LICENSE` & `brother_printer_fwupd-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.1/brother_printer_fwupd/__main__.py` & `brother_printer_fwupd-0.5.2/brother_printer_fwupd/__main__.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.1/brother_printer_fwupd/autodiscover_printer.py` & `brother_printer_fwupd-0.5.2/brother_printer_fwupd/autodiscover_printer.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.1/brother_printer_fwupd/firmware_downloader.py` & `brother_printer_fwupd-0.5.2/brother_printer_fwupd/firmware_downloader.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.1/brother_printer_fwupd/firmware_uploader.py` & `brother_printer_fwupd-0.5.2/brother_printer_fwupd/firmware_uploader.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.1/brother_printer_fwupd/models.py` & `brother_printer_fwupd-0.5.2/brother_printer_fwupd/models.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.1/brother_printer_fwupd/snmp_info.py` & `brother_printer_fwupd-0.5.2/brother_printer_fwupd/snmp_info.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.1/brother_printer_fwupd/utils.py` & `brother_printer_fwupd-0.5.2/brother_printer_fwupd/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,20 +44,15 @@
 
     def __enter__(self):
         self._handler.stream.seek(0)
         self._handler.stream.truncate()
         self.logger.addHandler(self._handler)
 
     def __exit__(self, exc_class, exc, tb):
-        #  breakpoint()
-        #  sys.stdout = self._std_out
-        #  sys.stderr = self._std_err
-        #  sys.stdin = self._std_in
-
-        if not exc_class:
+        if not exc_class or exc_class is SystemExit:
             return
 
         LOGGER.error(exc)
         self.logger.removeHandler(self._handler)
         self._handler.stream.seek(0)
         log_output = self._handler.stream.read()
         prog = Path(sys.argv[0]).name
```

### Comparing `brother_printer_fwupd-0.5.1/pyproject.toml` & `brother_printer_fwupd-0.5.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brother_printer_fwupd"
-version = "0.5.1"
+version = "0.5.2"
 description = "Script to update the firmware of some Brother printers (e. g. MFC)."
 authors = ["sedrubal <dev@sedrubal.de>"]
 repository = "https://github.com/sedrubal/brother_printer_fwupd.git"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `brother_printer_fwupd-0.5.1/PKG-INFO` & `brother_printer_fwupd-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brother-printer-fwupd
-Version: 0.5.1
+Version: 0.5.2
 Summary: Script to update the firmware of some Brother printers (e. g. MFC).
 Home-page: https://github.com/sedrubal/brother_printer_fwupd.git
 License: GPL-3.0-or-later
 Author: sedrubal
 Author-email: dev@sedrubal.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

