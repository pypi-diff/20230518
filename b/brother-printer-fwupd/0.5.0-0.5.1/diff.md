# Comparing `tmp/brother_printer_fwupd-0.5.0.tar.gz` & `tmp/brother_printer_fwupd-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brother_printer_fwupd-0.5.0.tar", max compression
+gzip compressed data, was "brother_printer_fwupd-0.5.1.tar", max compression
```

## Comparing `brother_printer_fwupd-0.5.0.tar` & `brother_printer_fwupd-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35150 2019-05-05 22:45:01.929067 brother_printer_fwupd-0.5.0/LICENSE
--rw-r--r--   0        0        0       75 2022-06-04 19:12:12.377682 brother_printer_fwupd-0.5.0/brother_printer_fwupd/__init__.py
--rwxr-xr-x   0        0        0     6098 2023-05-18 13:36:05.427176 brother_printer_fwupd-0.5.0/brother_printer_fwupd/__main__.py
--rw-r--r--   0        0        0     7080 2023-05-18 13:19:45.294187 brother_printer_fwupd-0.5.0/brother_printer_fwupd/autodiscover_printer.py
--rw-r--r--   0        0        0     3128 2023-05-18 13:19:29.797478 brother_printer_fwupd-0.5.0/brother_printer_fwupd/firmware_downloader.py
--rw-r--r--   0        0        0      739 2023-05-18 11:50:56.235324 brother_printer_fwupd-0.5.0/brother_printer_fwupd/firmware_uploader.py
--rw-r--r--   0        0        0     1718 2023-05-18 11:55:02.716491 brother_printer_fwupd-0.5.0/brother_printer_fwupd/models.py
--rw-r--r--   0        0        0     3050 2022-06-04 20:30:23.818775 brother_printer_fwupd-0.5.0/brother_printer_fwupd/snmp_info.py
--rw-r--r--   0        0        0     5853 2023-05-18 13:37:45.074134 brother_printer_fwupd-0.5.0/brother_printer_fwupd/utils.py
--rw-r--r--   0        0        0      875 2023-05-18 11:31:53.701264 brother_printer_fwupd-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 brother_printer_fwupd-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35150 2019-05-05 22:45:01.929067 brother_printer_fwupd-0.5.1/LICENSE
+-rw-r--r--   0        0        0       75 2022-06-04 19:12:12.377682 brother_printer_fwupd-0.5.1/brother_printer_fwupd/__init__.py
+-rwxr-xr-x   0        0        0     6212 2023-05-18 13:46:41.285683 brother_printer_fwupd-0.5.1/brother_printer_fwupd/__main__.py
+-rw-r--r--   0        0        0     7080 2023-05-18 13:19:45.294187 brother_printer_fwupd-0.5.1/brother_printer_fwupd/autodiscover_printer.py
+-rw-r--r--   0        0        0     3128 2023-05-18 13:19:29.797478 brother_printer_fwupd-0.5.1/brother_printer_fwupd/firmware_downloader.py
+-rw-r--r--   0        0        0      739 2023-05-18 11:50:56.235324 brother_printer_fwupd-0.5.1/brother_printer_fwupd/firmware_uploader.py
+-rw-r--r--   0        0        0     1718 2023-05-18 11:55:02.716491 brother_printer_fwupd-0.5.1/brother_printer_fwupd/models.py
+-rw-r--r--   0        0        0     3050 2022-06-04 20:30:23.818775 brother_printer_fwupd-0.5.1/brother_printer_fwupd/snmp_info.py
+-rw-r--r--   0        0        0     5853 2023-05-18 13:37:45.074134 brother_printer_fwupd-0.5.1/brother_printer_fwupd/utils.py
+-rw-r--r--   0        0        0      875 2023-05-18 13:47:29.349154 brother_printer_fwupd-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 brother_printer_fwupd-0.5.1/PKG-INFO
```

### Comparing `brother_printer_fwupd-0.5.0/LICENSE` & `brother_printer_fwupd-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.0/brother_printer_fwupd/__main__.py` & `brother_printer_fwupd-0.5.1/brother_printer_fwupd/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -169,18 +169,17 @@
             printer_ip = mdns_printer_info.ip_addr
             upload_port = mdns_printer_info.port
 
     if not printer_ip and printer_ip_required:
         LOGGER.critical("No printer given or found.")
         sys.exit(1)
 
-    assert printer_ip
-
     if use_snmp:
         LOGGER.info("Querying printer info via SNMP.")
+        assert printer_ip, "Printer IP is required but not given."
         printer_info = get_snmp_info(target=printer_ip, community=args.community)
     else:
         printer_info = SNMPPrinterInfo(
             model=args.model,
             serial=args.serial,
             spec=args.spec,
             fw_versions=args.fw_versions,
@@ -210,14 +209,15 @@
         LOGGER.success("Downloading firmware file.")
         download_fw(url=download_url, dst=args.fw_file)
 
         if args.download_only:
             LOGGER.info("Skipping firmware upload due to --download-only")
         else:
             LOGGER.info("Uploading firmware file to printer via jetdirect.")
+            assert printer_ip, "Printer IP is required but not given"
             upload_fw(target=printer_ip, port=upload_port, file_path=args.fw_file)
             input("Continue? ")
 
     LOGGER.success("Done.")
 
 
 if __name__ == "__main__":
```

### Comparing `brother_printer_fwupd-0.5.0/brother_printer_fwupd/autodiscover_printer.py` & `brother_printer_fwupd-0.5.1/brother_printer_fwupd/autodiscover_printer.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.0/brother_printer_fwupd/firmware_downloader.py` & `brother_printer_fwupd-0.5.1/brother_printer_fwupd/firmware_downloader.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.0/brother_printer_fwupd/firmware_uploader.py` & `brother_printer_fwupd-0.5.1/brother_printer_fwupd/firmware_uploader.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.0/brother_printer_fwupd/models.py` & `brother_printer_fwupd-0.5.1/brother_printer_fwupd/models.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.0/brother_printer_fwupd/snmp_info.py` & `brother_printer_fwupd-0.5.1/brother_printer_fwupd/snmp_info.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.0/brother_printer_fwupd/utils.py` & `brother_printer_fwupd-0.5.1/brother_printer_fwupd/utils.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.5.0/pyproject.toml` & `brother_printer_fwupd-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brother_printer_fwupd"
-version = "0.5.0"
+version = "0.5.1"
 description = "Script to update the firmware of some Brother printers (e. g. MFC)."
 authors = ["sedrubal <dev@sedrubal.de>"]
 repository = "https://github.com/sedrubal/brother_printer_fwupd.git"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `brother_printer_fwupd-0.5.0/PKG-INFO` & `brother_printer_fwupd-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brother-printer-fwupd
-Version: 0.5.0
+Version: 0.5.1
 Summary: Script to update the firmware of some Brother printers (e. g. MFC).
 Home-page: https://github.com/sedrubal/brother_printer_fwupd.git
 License: GPL-3.0-or-later
 Author: sedrubal
 Author-email: dev@sedrubal.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

