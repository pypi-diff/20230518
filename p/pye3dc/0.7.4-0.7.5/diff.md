# Comparing `tmp/pye3dc-0.7.4.tar.gz` & `tmp/pye3dc-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pye3dc-0.7.4.tar", last modified: Wed Feb  1 23:05:47 2023, max compression
+gzip compressed data, was "pye3dc-0.7.5.tar", last modified: Thu May 18 10:05:56 2023, max compression
```

## Comparing `pye3dc-0.7.4.tar` & `pye3dc-0.7.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 23:05:47.201611 pye3dc-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-01 23:05:45.000000 pye3dc-0.7.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-02-01 23:05:45.000000 pye3dc-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-02-01 23:05:47.201611 pye3dc-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-02-01 23:05:45.000000 pye3dc-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 23:05:47.201611 pye3dc-0.7.4/e3dc/
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-02-01 23:05:45.000000 pye3dc-0.7.4/e3dc/_RSCPEncryptDecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-01 23:05:45.000000 pye3dc-0.7.4/e3dc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84384 2023-02-01 23:05:45.000000 pye3dc-0.7.4/e3dc/_e3dc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-02-01 23:05:45.000000 pye3dc-0.7.4/e3dc/_e3dc_rscp_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-02-01 23:05:45.000000 pye3dc-0.7.4/e3dc/_e3dc_rscp_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-02-01 23:05:45.000000 pye3dc-0.7.4/e3dc/_rscpLib.py
--rw-r--r--   0 runner    (1001) docker     (123)    85445 2023-02-01 23:05:45.000000 pye3dc-0.7.4/e3dc/_rscpTags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 23:05:47.201611 pye3dc-0.7.4/pye3dc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-02-01 23:05:47.000000 pye3dc-0.7.4/pye3dc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-02-01 23:05:47.000000 pye3dc-0.7.4/pye3dc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 23:05:47.000000 pye3dc-0.7.4/pye3dc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 23:05:47.000000 pye3dc-0.7.4/pye3dc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-01 23:05:47.000000 pye3dc-0.7.4/pye3dc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-01 23:05:47.000000 pye3dc-0.7.4/pye3dc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-01 23:05:45.000000 pye3dc-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-02-01 23:05:47.205611 pye3dc-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-01 23:05:45.000000 pye3dc-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:05:55.996373 pye3dc-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 10:05:55.000000 pye3dc-0.7.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-18 10:05:55.000000 pye3dc-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-18 10:05:55.996373 pye3dc-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-18 10:05:55.000000 pye3dc-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:05:55.992373 pye3dc-0.7.5/e3dc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-18 10:05:55.000000 pye3dc-0.7.5/e3dc/_RSCPEncryptDecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-18 10:05:55.000000 pye3dc-0.7.5/e3dc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84325 2023-05-18 10:05:55.000000 pye3dc-0.7.5/e3dc/_e3dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-18 10:05:55.000000 pye3dc-0.7.5/e3dc/_e3dc_rscp_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-05-18 10:05:55.000000 pye3dc-0.7.5/e3dc/_e3dc_rscp_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-18 10:05:55.000000 pye3dc-0.7.5/e3dc/_rscpLib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85445 2023-05-18 10:05:55.000000 pye3dc-0.7.5/e3dc/_rscpTags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:05:55.996373 pye3dc-0.7.5/pye3dc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-18 10:05:55.000000 pye3dc-0.7.5/pye3dc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-18 10:05:55.000000 pye3dc-0.7.5/pye3dc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:05:55.000000 pye3dc-0.7.5/pye3dc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:05:55.000000 pye3dc-0.7.5/pye3dc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 10:05:55.000000 pye3dc-0.7.5/pye3dc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 10:05:55.000000 pye3dc-0.7.5/pye3dc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-18 10:05:55.000000 pye3dc-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-18 10:05:55.996373 pye3dc-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 10:05:55.000000 pye3dc-0.7.5/setup.py
```

### Comparing `pye3dc-0.7.4/LICENSE` & `pye3dc-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pye3dc-0.7.4/PKG-INFO` & `pye3dc-0.7.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pye3dc
-Version: 0.7.4
+Version: 0.7.5
 Summary: E3/DC client for python.
 Home-page: https://github.com/fsantini/python-e3dc
 Author: Francesco Santini
 Author-email: francesco.santini@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -22,14 +22,15 @@
 License-File: AUTHORS
 
 # python-e3dc
 
 [![PyPI version](https://badge.fury.io/py/pye3dc.svg)](https://badge.fury.io/py/pye3dc)
 [![GitHub license](https://img.shields.io/github/license/fsantini/python-e3dc)](https://github.com/fsantini/python-e3dc/blob/master/LICENSE)
 [![Codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/python-e3dc/badge/?version=latest)](https://python-e3dc.readthedocs.io/en/latest/?badge=latest)
 
 **NOTE: With Release 0.6.0 at least Python 3.7 is required**
 
 Python API for querying an [E3/DC](https://e3dc.de/) systems
 
 This is supported either directly via RSCP connection or through the manufacturer's portal. The RSCP implementation has currently the most capabilities.
 
@@ -143,15 +144,15 @@
 * `get_powermeter_data()`
 * `get_powermeters_data()`
 * `get_power_settings()`
 * `set_power_limits()`
 * `set_powersave()`
 * `set_weather_regulated_charge()`
 
-> A documentation for these methods is not yet generated. Please have a look at the docstrings in  `_e3dc.py` for details.
+See the full documentation on [ReadTheDocs](https://python-e3dc.readthedocs.io/en/latest/)
 
 ### Note: The RSCP interface
 
 The communication to an E3/DC system has to be implemented via a rather complicated protocol, called by E3/DC RSCP. This protocol is binary and based on websockets. The documentation provided by E3/DC is limited and outdated. It can be found in the E3/DC download portal.
 
 If keepAlive is false, the websocket connection is closed after the command. This makes sense because these requests are not meant to be made as often as the status requests, however, if keepAlive is True, the connection is left open and kept alive in the background in a separate thread.
 
@@ -189,11 +190,7 @@
 
 ## Contribution
 
 * open an issue before making a pull request
 * note the E3/DC system you tested with and implementation details
 * pull request checks will enforce code styling (black, flake8, isort)
 * consider adding yourself to `AUTHORS`
-
-## Copyright notice
-
-The Rijndael algorithm comes from the python-cryptoplus package by Philippe Teuwen (https://github.com/doegox/python-cryptoplus) and distributed under a MIT license.
```

### Comparing `pye3dc-0.7.4/README.md` & `pye3dc-0.7.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # python-e3dc
 
 [![PyPI version](https://badge.fury.io/py/pye3dc.svg)](https://badge.fury.io/py/pye3dc)
 [![GitHub license](https://img.shields.io/github/license/fsantini/python-e3dc)](https://github.com/fsantini/python-e3dc/blob/master/LICENSE)
 [![Codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/python-e3dc/badge/?version=latest)](https://python-e3dc.readthedocs.io/en/latest/?badge=latest)
 
 **NOTE: With Release 0.6.0 at least Python 3.7 is required**
 
 Python API for querying an [E3/DC](https://e3dc.de/) systems
 
 This is supported either directly via RSCP connection or through the manufacturer's portal. The RSCP implementation has currently the most capabilities.
 
@@ -120,15 +121,15 @@
 * `get_powermeter_data()`
 * `get_powermeters_data()`
 * `get_power_settings()`
 * `set_power_limits()`
 * `set_powersave()`
 * `set_weather_regulated_charge()`
 
-> A documentation for these methods is not yet generated. Please have a look at the docstrings in  `_e3dc.py` for details.
+See the full documentation on [ReadTheDocs](https://python-e3dc.readthedocs.io/en/latest/)
 
 ### Note: The RSCP interface
 
 The communication to an E3/DC system has to be implemented via a rather complicated protocol, called by E3/DC RSCP. This protocol is binary and based on websockets. The documentation provided by E3/DC is limited and outdated. It can be found in the E3/DC download portal.
 
 If keepAlive is false, the websocket connection is closed after the command. This makes sense because these requests are not meant to be made as often as the status requests, however, if keepAlive is True, the connection is left open and kept alive in the background in a separate thread.
 
@@ -166,11 +167,7 @@
 
 ## Contribution
 
 * open an issue before making a pull request
 * note the E3/DC system you tested with and implementation details
 * pull request checks will enforce code styling (black, flake8, isort)
 * consider adding yourself to `AUTHORS`
-
-## Copyright notice
-
-The Rijndael algorithm comes from the python-cryptoplus package by Philippe Teuwen (https://github.com/doegox/python-cryptoplus) and distributed under a MIT license.
```

### Comparing `pye3dc-0.7.4/e3dc/_RSCPEncryptDecrypt.py` & `pye3dc-0.7.5/e3dc/_RSCPEncryptDecrypt.py`

 * *Files identical despite different names*

### Comparing `pye3dc-0.7.4/e3dc/_e3dc.py` & `pye3dc-0.7.5/e3dc/_e3dc.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
         if self.serialNumber.startswith("4") or self.serialNumber.startswith("72"):
             self.model = "S10E"
             self.powermeters = self.powermeters or [{"index": 0}]
             self.pvis = self.pvis or [{"index": 0}]
             if not self.serialNumberPrefix:
                 self.serialNumberPrefix = "S10-"
-        if self.serialNumber.startswith("74"):
+        elif self.serialNumber.startswith("74"):
             self.model = "S10E_Compact"
             self.powermeters = self.powermeters or [{"index": 0}]
             self.pvis = self.pvis or [{"index": 0}]
             if not self.serialNumberPrefix:
                 self.serialNumberPrefix = "S10-"
         elif self.serialNumber.startswith("5"):
             self.model = "S10_Mini"
@@ -1980,35 +1980,33 @@
             enable (bool): True/False
             keepAlive (Optional[bool]): True to keep connection alive
 
         Returns:
             0 if success
             -1 if error
         """
-        if enable:
-            res = self.sendRequest(
-                (
-                    "EMS_REQ_SET_POWER_SETTINGS",
-                    "Container",
-                    [("EMS_POWERSAVE_ENABLED", "UChar8", 1)],
-                ),
-                keepAlive=keepAlive,
-            )
-        else:
-            res = self.sendRequest(
-                (
-                    "EMS_REQ_SET_POWER_SETTINGS",
-                    "Container",
-                    [("EMS_POWERSAVE_ENABLED", "UChar8", 0)],
-                ),
-                keepAlive=keepAlive,
-            )
+        res = self.sendRequest(
+            (
+                "EMS_REQ_SET_POWER_SETTINGS",
+                "Container",
+                [("EMS_POWERSAVE_ENABLED", "UChar8", int(enable))],
+            ),
+            keepAlive=keepAlive,
+        )
+
+        # Returns value of EMS_REQ_SET_POWER_SETTINGS, we get a success flag here,
+        # that we normalize and push outside.
+        # [ "EMS_SET_POWER_SETTINGS",
+        #   "Container",
+        #   [
+        #       ["EMS_RES_POWERSAVE_ENABLED", "Char8", 0]
+        #   ]
+        # ]
 
-        # validate return code for EMS_RES_POWERSAVE_ENABLED is 0
-        if res[2][0][2] == 0:
+        if rscpFindTagIndex(res, "EMS_RES_POWERSAVE_ENABLED") == 0:
             return 0
         else:
             return -1
 
     def set_weather_regulated_charge(self, enable, keepAlive=False):
         """Setting the SmartCharge weather regulated charge via rscp protocol locally.
```

### Comparing `pye3dc-0.7.4/e3dc/_e3dc_rscp_local.py` & `pye3dc-0.7.5/e3dc/_e3dc_rscp_local.py`

 * *Files identical despite different names*

### Comparing `pye3dc-0.7.4/e3dc/_e3dc_rscp_web.py` & `pye3dc-0.7.5/e3dc/_e3dc_rscp_web.py`

 * *Files identical despite different names*

### Comparing `pye3dc-0.7.4/e3dc/_rscpLib.py` & `pye3dc-0.7.5/e3dc/_rscpLib.py`

 * *Files identical despite different names*

### Comparing `pye3dc-0.7.4/e3dc/_rscpTags.py` & `pye3dc-0.7.5/e3dc/_rscpTags.py`

 * *Files identical despite different names*

### Comparing `pye3dc-0.7.4/pye3dc.egg-info/PKG-INFO` & `pye3dc-0.7.5/pye3dc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pye3dc
-Version: 0.7.4
+Version: 0.7.5
 Summary: E3/DC client for python.
 Home-page: https://github.com/fsantini/python-e3dc
 Author: Francesco Santini
 Author-email: francesco.santini@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -22,14 +22,15 @@
 License-File: AUTHORS
 
 # python-e3dc
 
 [![PyPI version](https://badge.fury.io/py/pye3dc.svg)](https://badge.fury.io/py/pye3dc)
 [![GitHub license](https://img.shields.io/github/license/fsantini/python-e3dc)](https://github.com/fsantini/python-e3dc/blob/master/LICENSE)
 [![Codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/python-e3dc/badge/?version=latest)](https://python-e3dc.readthedocs.io/en/latest/?badge=latest)
 
 **NOTE: With Release 0.6.0 at least Python 3.7 is required**
 
 Python API for querying an [E3/DC](https://e3dc.de/) systems
 
 This is supported either directly via RSCP connection or through the manufacturer's portal. The RSCP implementation has currently the most capabilities.
 
@@ -143,15 +144,15 @@
 * `get_powermeter_data()`
 * `get_powermeters_data()`
 * `get_power_settings()`
 * `set_power_limits()`
 * `set_powersave()`
 * `set_weather_regulated_charge()`
 
-> A documentation for these methods is not yet generated. Please have a look at the docstrings in  `_e3dc.py` for details.
+See the full documentation on [ReadTheDocs](https://python-e3dc.readthedocs.io/en/latest/)
 
 ### Note: The RSCP interface
 
 The communication to an E3/DC system has to be implemented via a rather complicated protocol, called by E3/DC RSCP. This protocol is binary and based on websockets. The documentation provided by E3/DC is limited and outdated. It can be found in the E3/DC download portal.
 
 If keepAlive is false, the websocket connection is closed after the command. This makes sense because these requests are not meant to be made as often as the status requests, however, if keepAlive is True, the connection is left open and kept alive in the background in a separate thread.
 
@@ -189,11 +190,7 @@
 
 ## Contribution
 
 * open an issue before making a pull request
 * note the E3/DC system you tested with and implementation details
 * pull request checks will enforce code styling (black, flake8, isort)
 * consider adding yourself to `AUTHORS`
-
-## Copyright notice
-
-The Rijndael algorithm comes from the python-cryptoplus package by Philippe Teuwen (https://github.com/doegox/python-cryptoplus) and distributed under a MIT license.
```

### Comparing `pye3dc-0.7.4/setup.cfg` & `pye3dc-0.7.5/setup.cfg`

 * *Files identical despite different names*

