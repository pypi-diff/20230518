# Comparing `tmp/slixmpp-omemo-0.9.0.tar.gz` & `tmp/slixmpp-omemo-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slixmpp-omemo-0.9.0.tar", last modified: Sun Jan  1 18:14:43 2023, max compression
+gzip compressed data, was "slixmpp-omemo-0.9.1.tar", last modified: Thu May 18 13:56:51 2023, max compression
```

## Comparing `slixmpp-omemo-0.9.0.tar` & `slixmpp-omemo-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2023-01-01 18:14:43.882814 slixmpp-omemo-0.9.0/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    35148 2019-02-17 17:36:43.000000 slixmpp-omemo-0.9.0/LICENSE
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2297 2023-01-01 18:14:43.882814 slixmpp-omemo-0.9.0/PKG-INFO
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1500 2022-03-12 00:33:10.000000 slixmpp-omemo-0.9.0/README.rst
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       38 2023-01-01 18:14:43.882814 slixmpp-omemo-0.9.0/setup.cfg
--rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     1884 2023-01-01 18:14:41.000000 slixmpp-omemo-0.9.0/setup.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2023-01-01 18:14:43.879481 slixmpp-omemo-0.9.0/slixmpp_omemo/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)    32843 2023-01-01 18:14:41.000000 slixmpp-omemo-0.9.0/slixmpp_omemo/__init__.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)        0 2022-03-24 14:55:28.000000 slixmpp-omemo-0.9.0/slixmpp_omemo/py.typed
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      744 2022-11-14 21:32:14.000000 slixmpp-omemo-0.9.0/slixmpp_omemo/rewrite.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4346 2019-08-22 17:24:29.000000 slixmpp-omemo-0.9.0/slixmpp_omemo/stanza.py
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      286 2023-01-01 18:14:41.000000 slixmpp-omemo-0.9.0/slixmpp_omemo/version.py
-drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2023-01-01 18:14:43.882814 slixmpp-omemo-0.9.0/slixmpp_omemo.egg-info/
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2297 2023-01-01 18:14:43.000000 slixmpp-omemo-0.9.0/slixmpp_omemo.egg-info/PKG-INFO
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)      334 2023-01-01 18:14:43.000000 slixmpp-omemo-0.9.0/slixmpp_omemo.egg-info/SOURCES.txt
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)        1 2023-01-01 18:14:43.000000 slixmpp-omemo-0.9.0/slixmpp_omemo.egg-info/dependency_links.txt
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       63 2023-01-01 18:14:43.000000 slixmpp-omemo-0.9.0/slixmpp_omemo.egg-info/requires.txt
--rw-r--r--   0 ppjet     (1000) ppjet     (1000)       14 2023-01-01 18:14:43.000000 slixmpp-omemo-0.9.0/slixmpp_omemo.egg-info/top_level.txt
+drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2023-05-18 13:56:51.730842 slixmpp-omemo-0.9.1/
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)    35148 2019-02-17 17:36:43.000000 slixmpp-omemo-0.9.1/LICENSE
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2297 2023-05-18 13:56:51.730842 slixmpp-omemo-0.9.1/PKG-INFO
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)     1500 2022-03-12 00:33:10.000000 slixmpp-omemo-0.9.1/README.rst
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)       38 2023-05-18 13:56:51.730842 slixmpp-omemo-0.9.1/setup.cfg
+-rwxr-xr-x   0 ppjet     (1000) ppjet     (1000)     1884 2023-01-01 18:14:41.000000 slixmpp-omemo-0.9.1/setup.py
+drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2023-05-18 13:56:51.730842 slixmpp-omemo-0.9.1/slixmpp_omemo/
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)    32749 2023-05-18 13:52:24.000000 slixmpp-omemo-0.9.1/slixmpp_omemo/__init__.py
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)        0 2022-03-24 14:55:28.000000 slixmpp-omemo-0.9.1/slixmpp_omemo/py.typed
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)      744 2022-11-14 21:32:14.000000 slixmpp-omemo-0.9.1/slixmpp_omemo/rewrite.py
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)     4346 2019-08-22 17:24:29.000000 slixmpp-omemo-0.9.1/slixmpp_omemo/stanza.py
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)      286 2023-05-18 13:54:44.000000 slixmpp-omemo-0.9.1/slixmpp_omemo/version.py
+drwxr-xr-x   0 ppjet     (1000) ppjet     (1000)        0 2023-05-18 13:56:51.730842 slixmpp-omemo-0.9.1/slixmpp_omemo.egg-info/
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)     2297 2023-05-18 13:56:51.000000 slixmpp-omemo-0.9.1/slixmpp_omemo.egg-info/PKG-INFO
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)      334 2023-05-18 13:56:51.000000 slixmpp-omemo-0.9.1/slixmpp_omemo.egg-info/SOURCES.txt
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)        1 2023-05-18 13:56:51.000000 slixmpp-omemo-0.9.1/slixmpp_omemo.egg-info/dependency_links.txt
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)       63 2023-05-18 13:56:51.000000 slixmpp-omemo-0.9.1/slixmpp_omemo.egg-info/requires.txt
+-rw-r--r--   0 ppjet     (1000) ppjet     (1000)       14 2023-05-18 13:56:51.000000 slixmpp-omemo-0.9.1/slixmpp_omemo.egg-info/top_level.txt
```

### Comparing `slixmpp-omemo-0.9.0/LICENSE` & `slixmpp-omemo-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slixmpp-omemo-0.9.0/PKG-INFO` & `slixmpp-omemo-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slixmpp-omemo
-Version: 0.9.0
+Version: 0.9.1
 Summary: Slixmpp OMEMO plugin
 Home-page: https://lab.louiz.org/poezio/slixmpp-omemo
 Author: Maxime Buquet
 Author-email: pep@bouah.net
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `slixmpp-omemo-0.9.0/README.rst` & `slixmpp-omemo-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `slixmpp-omemo-0.9.0/setup.py` & `slixmpp-omemo-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `slixmpp-omemo-0.9.0/slixmpp_omemo/__init__.py` & `slixmpp-omemo-0.9.1/slixmpp_omemo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,34 +232,33 @@
             raise PluginCouldNotLoad
 
         if not self.data_dir:
             raise PluginCouldNotLoad("xep_0384 cannot be loaded as there is "
                                      "no data directory specified.")
 
         self._device_id = _load_device_id(self.data_dir)
-        asyncio.create_task(self.session_start_omemo())
 
         self.xmpp.add_event_handler('session_start', self.session_start)
         self.xmpp['xep_0060'].map_node_event(OMEMO_DEVICES_NS, 'omemo_device_list')
         self.xmpp.add_event_handler('omemo_device_list_publish', self._receive_device_list)
 
         # If this plugin is loaded after 'session_start' has fired, we still
         # need to publish bundles
         if self.xmpp.is_connected and not self._initial_publish_done:
-            asyncio.create_task(self._initial_publish())
+            asyncio.ensure_future(self.session_start(None))
 
     def plugin_end(self):
         if not self.backend_loaded:
             return
 
         self.xmpp.remove_event_handler('session_start', self.session_start)
         self.xmpp.remove_event_handler('omemo_device_list_publish', self._receive_device_list)
         self.xmpp['xep_0163'].remove_interest(OMEMO_DEVICES_NS)
 
-    async def session_start_omemo(self):
+    async def session_start(self, _jid):
         """Creates the OMEMO session object"""
 
         storage = self.storage_backend
         if self.storage_backend is None:
             storage = JSONFileStorage(self.data_dir)
 
         otpkpolicy = self.otpk_policy
@@ -273,23 +272,22 @@
                 bare_jid,
                 self._device_id,
             )
         except Exception as exn:
             log.error("Couldn't load the OMEMO object; ¯\\_(ツ)_/¯")
             raise PluginCouldNotLoad from exn
 
+        await self._initial_publish()
+
     def _omemo(self) -> SessionManager:
         """Helper method to unguard potentially uninitialized SessionManager"""
         if self.__omemo_session is None:
             raise UninitializedOMEMOSession
         return self.__omemo_session
 
-    async def session_start(self, _jid):
-        await self._initial_publish()
-
     async def _initial_publish(self):
         if self.backend_loaded:
             self.xmpp['xep_0163'].add_interest(OMEMO_DEVICES_NS)
             await asyncio.wait([
                 asyncio.create_task(self._set_device_list()),
                 asyncio.create_task(self._publish_bundle()),
             ])
```

### Comparing `slixmpp-omemo-0.9.0/slixmpp_omemo/rewrite.py` & `slixmpp-omemo-0.9.1/slixmpp_omemo/rewrite.py`

 * *Files identical despite different names*

### Comparing `slixmpp-omemo-0.9.0/slixmpp_omemo/stanza.py` & `slixmpp-omemo-0.9.1/slixmpp_omemo/stanza.py`

 * *Files identical despite different names*

### Comparing `slixmpp-omemo-0.9.0/slixmpp_omemo.egg-info/PKG-INFO` & `slixmpp-omemo-0.9.1/slixmpp_omemo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slixmpp-omemo
-Version: 0.9.0
+Version: 0.9.1
 Summary: Slixmpp OMEMO plugin
 Home-page: https://lab.louiz.org/poezio/slixmpp-omemo
 Author: Maxime Buquet
 Author-email: pep@bouah.net
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

