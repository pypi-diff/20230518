# Comparing `tmp/wg-easy-api-wrapper-1.0.1.tar.gz` & `tmp/wg-easy-api-wrapper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg-easy-api-wrapper-1.0.1.tar", last modified: Wed May 17 22:08:52 2023, max compression
+gzip compressed data, was "wg-easy-api-wrapper-1.0.2.tar", last modified: Wed May 17 22:28:33 2023, max compression
```

## Comparing `wg-easy-api-wrapper-1.0.1.tar` & `wg-easy-api-wrapper-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:08:52.366329 wg-easy-api-wrapper-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 22:08:52.366329 wg-easy-api-wrapper-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-17 22:08:43.000000 wg-easy-api-wrapper-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-17 22:08:52.370329 wg-easy-api-wrapper-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:08:43.000000 wg-easy-api-wrapper-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:08:52.366329 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 22:08:43.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-17 22:08:43.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-17 22:08:43.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:08:52.366329 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 22:08:52.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-17 22:08:52.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:08:52.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 22:08:52.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-17 22:08:52.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:28:33.787729 wg-easy-api-wrapper-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 22:28:33.787729 wg-easy-api-wrapper-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-17 22:28:26.000000 wg-easy-api-wrapper-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-17 22:28:33.787729 wg-easy-api-wrapper-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:28:26.000000 wg-easy-api-wrapper-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:28:33.783729 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 22:28:26.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-17 22:28:26.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-17 22:28:26.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:28:33.787729 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 22:28:33.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-17 22:28:33.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:28:33.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 22:28:33.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-17 22:28:33.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/top_level.txt
```

### Comparing `wg-easy-api-wrapper-1.0.1/PKG-INFO` & `wg-easy-api-wrapper-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-easy-api-wrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wrapper for wg-easy API
 Home-page: https://github.com/Shandeika/wg-easy-api-wrapper
 Author: MrShandy
 Author-email: mrshandy@shandy-dev.ru
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `wg-easy-api-wrapper-1.0.1/setup.cfg` & `wg-easy-api-wrapper-1.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wg-easy-api-wrapper
-version = 1.0.1
+version = 1.0.2
 author = MrShandy
 author_email = mrshandy@shandy-dev.ru
 description = Wrapper for wg-easy API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Shandeika/wg-easy-api-wrapper
 license = GPL-3.0
```

### Comparing `wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/client.py` & `wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,14 @@
                  persistent_keepalive: str,
                  public_key: str,
                  transfer_rx: int,
                  transfer_tx: int,
                  updated_at: str,
                  session: aiohttp.ClientSession,
                  server: 'Server',):
-        # вывод всех входящих аргументов
-        print(address, created_at, enabled, uid, last_handshake_at, name, persistent_keepalive, public_key, transfer_rx, transfer_tx, updated_at)
         self._address = address
         self._created_at = datetime.strptime(created_at, time_format)
         self._enabled = bool(enabled)
         self._uid = uid
         self._last_handshake_at = datetime.strptime(last_handshake_at, time_format) if last_handshake_at else None
         self._name = name
         self._persistent_keepalive = persistent_keepalive
```

### Comparing `wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/server.py` & `wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/server.py`

 * *Files identical despite different names*

### Comparing `wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/PKG-INFO` & `wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-easy-api-wrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wrapper for wg-easy API
 Home-page: https://github.com/Shandeika/wg-easy-api-wrapper
 Author: MrShandy
 Author-email: mrshandy@shandy-dev.ru
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

