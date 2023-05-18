# Comparing `tmp/pyrinnaitouch-0.9.2.tar.gz` & `tmp/pyrinnaitouch-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrinnaitouch-0.9.2.tar", last modified: Mon Mar 14 12:36:58 2022, max compression
+gzip compressed data, was "pyrinnaitouch-0.9.3.tar", last modified: Tue Dec 20 23:53:55 2022, max compression
```

## Comparing `pyrinnaitouch-0.9.2.tar` & `pyrinnaitouch-0.9.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 12:36:58.783831 pyrinnaitouch-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-03-14 12:36:47.000000 pyrinnaitouch-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-03-14 12:36:58.783831 pyrinnaitouch-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-03-14 12:36:47.000000 pyrinnaitouch-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 12:36:58.783831 pyrinnaitouch-0.9.2/pyrinnaitouch/
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-03-14 12:36:47.000000 pyrinnaitouch-0.9.2/pyrinnaitouch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4450 2022-03-14 12:36:47.000000 pyrinnaitouch-0.9.2/pyrinnaitouch/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     7886 2022-03-14 12:36:47.000000 pyrinnaitouch-0.9.2/pyrinnaitouch/cooler.py
--rw-r--r--   0 runner    (1001) docker     (121)     5932 2022-03-14 12:36:47.000000 pyrinnaitouch-0.9.2/pyrinnaitouch/evap.py
--rw-r--r--   0 runner    (1001) docker     (121)     8056 2022-03-14 12:36:47.000000 pyrinnaitouch-0.9.2/pyrinnaitouch/heater.py
--rw-r--r--   0 runner    (1001) docker     (121)    26194 2022-03-14 12:36:47.000000 pyrinnaitouch-0.9.2/pyrinnaitouch/system.py
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-03-14 12:36:47.000000 pyrinnaitouch-0.9.2/pyrinnaitouch/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 12:36:58.783831 pyrinnaitouch-0.9.2/pyrinnaitouch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-03-14 12:36:58.000000 pyrinnaitouch-0.9.2/pyrinnaitouch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-14 12:36:58.000000 pyrinnaitouch-0.9.2/pyrinnaitouch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-14 12:36:58.000000 pyrinnaitouch-0.9.2/pyrinnaitouch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-14 12:36:58.000000 pyrinnaitouch-0.9.2/pyrinnaitouch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-14 12:36:58.000000 pyrinnaitouch-0.9.2/pyrinnaitouch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-14 12:36:58.787831 pyrinnaitouch-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-03-14 12:36:47.000000 pyrinnaitouch-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 23:53:55.779084 pyrinnaitouch-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2022-12-20 23:53:43.000000 pyrinnaitouch-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2022-12-20 23:53:55.783084 pyrinnaitouch-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-20 23:53:43.000000 pyrinnaitouch-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 23:53:55.779084 pyrinnaitouch-0.9.3/pyrinnaitouch/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2022-12-20 23:53:43.000000 pyrinnaitouch-0.9.3/pyrinnaitouch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2022-12-20 23:53:43.000000 pyrinnaitouch-0.9.3/pyrinnaitouch/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2022-12-20 23:53:43.000000 pyrinnaitouch-0.9.3/pyrinnaitouch/cooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2022-12-20 23:53:43.000000 pyrinnaitouch-0.9.3/pyrinnaitouch/evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2022-12-20 23:53:43.000000 pyrinnaitouch-0.9.3/pyrinnaitouch/heater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26194 2022-12-20 23:53:43.000000 pyrinnaitouch-0.9.3/pyrinnaitouch/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2022-12-20 23:53:43.000000 pyrinnaitouch-0.9.3/pyrinnaitouch/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 23:53:55.779084 pyrinnaitouch-0.9.3/pyrinnaitouch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2022-12-20 23:53:55.000000 pyrinnaitouch-0.9.3/pyrinnaitouch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-20 23:53:55.000000 pyrinnaitouch-0.9.3/pyrinnaitouch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 23:53:55.000000 pyrinnaitouch-0.9.3/pyrinnaitouch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-20 23:53:55.000000 pyrinnaitouch-0.9.3/pyrinnaitouch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-20 23:53:55.000000 pyrinnaitouch-0.9.3/pyrinnaitouch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-20 23:53:55.783084 pyrinnaitouch-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2022-12-20 23:53:43.000000 pyrinnaitouch-0.9.3/setup.py
```

### Comparing `pyrinnaitouch-0.9.2/LICENSE` & `pyrinnaitouch-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrinnaitouch-0.9.2/PKG-INFO` & `pyrinnaitouch-0.9.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyrinnaitouch
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python interface to the Rinnai Touch Wifi controller
 Home-page: https://github.com/funtastix/pyrinnaitouch
 Download-URL: https://github.com/funtastix/pyrinnaitouch/archive/refs/tags/v0.9.0.tar.gz
 Author: Funtastix
 License: mit
 Keywords: Rinnai Touch,Brivis,IoT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: Topic :: System :: Hardware
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -36,9 +35,7 @@
 The aim of this package is to be used by software developers and integrators to implement
 the Rinnai Touch Wifi interface on home automation platforms (principally Home Assistant )
 
 ## Credit
 
 The [pescea interface](https://github.com/lazdavila/pescea) was used as a template and
 for inspiration in developing this library (which got it off to a good start, so thanks!)
-
-
```

### Comparing `pyrinnaitouch-0.9.2/README.md` & `pyrinnaitouch-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrinnaitouch-0.9.2/pyrinnaitouch/commands.py` & `pyrinnaitouch-0.9.3/pyrinnaitouch/commands.py`

 * *Files identical despite different names*

### Comparing `pyrinnaitouch-0.9.2/pyrinnaitouch/cooler.py` & `pyrinnaitouch-0.9.3/pyrinnaitouch/cooler.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 # Set temp?
                 set_temp = get_attribute(gso,"SP",None)
                 _LOGGER.debug("Cooling set temp is: %s", set_temp)
                 brivis_status.cooling_status.set_temp = int(set_temp)
 
                 brivis_status.cooling_status.set_advanced(get_attribute(gso,"AO",None))
 
-                gss = get_attribute(j[1].get("HGOM"),"GSS",None)
+                gss = get_attribute(j[1].get("CGOM"),"GSS",None)
                 if not gss:
                     _LOGGER.error("No GSS here")
                 else:
                     period = symbol_to_schedule_period(get_attribute(gss,"AT",None))
                     brivis_status.cooling_status.schedule_period = period
                     period = symbol_to_schedule_period(get_attribute(gss,"AZ",None))
                     brivis_status.cooling_status.advance_period = period
```

### Comparing `pyrinnaitouch-0.9.2/pyrinnaitouch/evap.py` & `pyrinnaitouch-0.9.3/pyrinnaitouch/evap.py`

 * *Files identical despite different names*

### Comparing `pyrinnaitouch-0.9.2/pyrinnaitouch/heater.py` & `pyrinnaitouch-0.9.3/pyrinnaitouch/heater.py`

 * *Files identical despite different names*

### Comparing `pyrinnaitouch-0.9.2/pyrinnaitouch/system.py` & `pyrinnaitouch-0.9.3/pyrinnaitouch/system.py`

 * *Files identical despite different names*

### Comparing `pyrinnaitouch-0.9.2/pyrinnaitouch/util.py` & `pyrinnaitouch-0.9.3/pyrinnaitouch/util.py`

 * *Files identical despite different names*

### Comparing `pyrinnaitouch-0.9.2/pyrinnaitouch.egg-info/PKG-INFO` & `pyrinnaitouch-0.9.3/pyrinnaitouch.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyrinnaitouch
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python interface to the Rinnai Touch Wifi controller
 Home-page: https://github.com/funtastix/pyrinnaitouch
 Download-URL: https://github.com/funtastix/pyrinnaitouch/archive/refs/tags/v0.9.0.tar.gz
 Author: Funtastix
 License: mit
 Keywords: Rinnai Touch,Brivis,IoT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: Topic :: System :: Hardware
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -36,9 +35,7 @@
 The aim of this package is to be used by software developers and integrators to implement
 the Rinnai Touch Wifi interface on home automation platforms (principally Home Assistant )
 
 ## Credit
 
 The [pescea interface](https://github.com/lazdavila/pescea) was used as a template and
 for inspiration in developing this library (which got it off to a good start, so thanks!)
-
-
```

### Comparing `pyrinnaitouch-0.9.2/setup.py` & `pyrinnaitouch-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as fh: # pylint: disable=unspecified-encoding
     LONG_DESCRIPTION = fh.read()
 
 setup(
     name="pyrinnaitouch",
     packages=find_packages(exclude=["tests", "tests.*"]),
-    version="0.9.2",
+    version="0.9.3",
     license="mit",
     description="A python interface to the Rinnai Touch Wifi controller",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author="Funtastix",
     url="https://github.com/funtastix/pyrinnaitouch",
     download_url="https://github.com/funtastix/pyrinnaitouch/archive/refs/tags/v0.9.0.tar.gz",
```

