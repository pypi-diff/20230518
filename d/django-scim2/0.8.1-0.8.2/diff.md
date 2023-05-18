# Comparing `tmp/django-scim2-0.8.1.tar.gz` & `tmp/django-scim2-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-scim2-0.8.1.tar", last modified: Tue Feb 26 21:47:18 2019, max compression
+gzip compressed data, was "dist/django-scim2-0.8.2.tar", last modified: Wed Feb 27 16:34:02 2019, max compression
```

## Comparing `django-scim2-0.8.1.tar` & `django-scim2-0.8.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-26 21:47:18.000000 django-scim2-0.8.1/
--rw-r--r--   0 paul       (501) staff       (20)     1337 2019-02-26 21:39:00.000000 django-scim2-0.8.1/CHANGES.txt
--rw-r--r--   0 paul       (501) staff       (20)     1211 2016-12-13 22:02:05.000000 django-scim2-0.8.1/LICENSE.txt
--rw-r--r--   0 paul       (501) staff       (20)      196 2016-12-29 07:31:06.000000 django-scim2-0.8.1/MANIFEST.in
--rw-r--r--   0 paul       (501) staff       (20)     4955 2019-02-26 21:47:18.000000 django-scim2-0.8.1/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     2892 2018-12-22 21:04:19.000000 django-scim2-0.8.1/README.rst
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-26 21:47:18.000000 django-scim2-0.8.1/django_scim/
--rw-r--r--   0 paul       (501) staff       (20)       22 2019-02-26 21:39:12.000000 django-scim2-0.8.1/django_scim/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)    13251 2019-02-25 19:03:30.000000 django-scim2-0.8.1/django_scim/adapters.py
--rw-r--r--   0 paul       (501) staff       (20)      804 2017-10-11 18:46:30.000000 django-scim2-0.8.1/django_scim/constants.py
--rw-r--r--   0 paul       (501) staff       (20)     1098 2018-12-13 23:14:02.000000 django-scim2-0.8.1/django_scim/exceptions.py
--rw-r--r--   0 paul       (501) staff       (20)    12426 2018-12-13 18:01:06.000000 django-scim2-0.8.1/django_scim/filters.py
--rw-r--r--   0 paul       (501) staff       (20)     2191 2018-12-13 18:01:06.000000 django-scim2-0.8.1/django_scim/grammars.py
--rw-r--r--   0 paul       (501) staff       (20)     2543 2019-02-21 06:10:50.000000 django-scim2-0.8.1/django_scim/middleware.py
--rw-r--r--   0 paul       (501) staff       (20)     7302 2019-02-26 03:40:17.000000 django-scim2-0.8.1/django_scim/models.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-26 21:47:18.000000 django-scim2-0.8.1/django_scim/schemas/
--rw-r--r--   0 paul       (501) staff       (20)      488 2016-12-13 22:02:05.000000 django-scim2-0.8.1/django_scim/schemas/README.rst
--rw-r--r--   0 paul       (501) staff       (20)      568 2017-03-09 00:06:19.000000 django-scim2-0.8.1/django_scim/schemas/__init__.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-26 21:47:18.000000 django-scim2-0.8.1/django_scim/schemas/core/
--rw-r--r--   0 paul       (501) staff       (20)     2051 2016-12-13 22:02:05.000000 django-scim2-0.8.1/django_scim/schemas/core/Group.json
--rw-r--r--   0 paul       (501) staff       (20)     3215 2016-12-13 22:02:05.000000 django-scim2-0.8.1/django_scim/schemas/core/ResourceType.json
--rw-r--r--   0 paul       (501) staff       (20)    11445 2016-12-13 22:02:05.000000 django-scim2-0.8.1/django_scim/schemas/core/Schema.json
--rw-r--r--   0 paul       (501) staff       (20)     6571 2016-12-13 22:02:05.000000 django-scim2-0.8.1/django_scim/schemas/core/ServiceProviderConfig.json
--rw-r--r--   0 paul       (501) staff       (20)    26634 2016-12-13 22:02:05.000000 django-scim2-0.8.1/django_scim/schemas/core/User.json
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-26 21:47:18.000000 django-scim2-0.8.1/django_scim/schemas/extension/
--rw-r--r--   0 paul       (501) staff       (20)     3426 2016-12-13 22:02:05.000000 django-scim2-0.8.1/django_scim/schemas/extension/Enterprise-User.json
--rw-r--r--   0 paul       (501) staff       (20)     4434 2018-12-13 18:55:45.000000 django-scim2-0.8.1/django_scim/settings.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-26 21:47:18.000000 django-scim2-0.8.1/django_scim/tests/
--rw-r--r--   0 paul       (501) staff       (20)        0 2016-12-13 22:02:05.000000 django-scim2-0.8.1/django_scim/tests/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)      537 2018-12-13 21:54:29.000000 django-scim2-0.8.1/django_scim/tests/hashers.py
--rw-r--r--   0 paul       (501) staff       (20)     8275 2019-02-26 21:35:11.000000 django-scim2-0.8.1/django_scim/tests/test_adapters.py
--rw-r--r--   0 paul       (501) staff       (20)     1055 2019-02-13 21:47:15.000000 django-scim2-0.8.1/django_scim/tests/test_grammar.py
--rw-r--r--   0 paul       (501) staff       (20)      592 2019-02-11 18:15:56.000000 django-scim2-0.8.1/django_scim/tests/test_middleware.py
--rw-r--r--   0 paul       (501) staff       (20)     1908 2019-02-26 21:33:11.000000 django-scim2-0.8.1/django_scim/tests/test_models.py
--rw-r--r--   0 paul       (501) staff       (20)      614 2017-07-25 21:53:37.000000 django-scim2-0.8.1/django_scim/tests/test_utils.py
--rw-r--r--   0 paul       (501) staff       (20)    33206 2019-02-13 20:01:01.000000 django-scim2-0.8.1/django_scim/tests/test_views.py
--rw-r--r--   0 paul       (501) staff       (20)      353 2018-06-13 17:08:36.000000 django-scim2-0.8.1/django_scim/tests/urls.py
--rw-r--r--   0 paul       (501) staff       (20)     1663 2018-12-13 18:01:06.000000 django-scim2-0.8.1/django_scim/urls.py
--rw-r--r--   0 paul       (501) staff       (20)     3505 2018-12-13 18:55:45.000000 django-scim2-0.8.1/django_scim/utils.py
--rw-r--r--   0 paul       (501) staff       (20)    14008 2019-02-21 21:30:47.000000 django-scim2-0.8.1/django_scim/views.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-26 21:47:18.000000 django-scim2-0.8.1/django_scim2.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     4955 2019-02-26 21:47:18.000000 django-scim2-0.8.1/django_scim2.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     1172 2019-02-26 21:47:18.000000 django-scim2-0.8.1/django_scim2.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2019-02-26 21:47:18.000000 django-scim2-0.8.1/django_scim2.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2018-06-12 21:20:24.000000 django-scim2-0.8.1/django_scim2.egg-info/not-zip-safe
--rw-r--r--   0 paul       (501) staff       (20)       42 2019-02-26 21:47:18.000000 django-scim2-0.8.1/django_scim2.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)       12 2019-02-26 21:47:18.000000 django-scim2-0.8.1/django_scim2.egg-info/top_level.txt
--rw-r--r--   0 paul       (501) staff       (20)       67 2019-02-26 21:47:18.000000 django-scim2-0.8.1/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)     2792 2019-02-26 21:37:48.000000 django-scim2-0.8.1/setup.py
--rw-r--r--   0 paul       (501) staff       (20)      398 2019-02-11 18:15:56.000000 django-scim2-0.8.1/tox.ini
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-27 16:34:02.000000 django-scim2-0.8.2/
+-rw-r--r--   0 paul       (501) staff       (20)     1380 2019-02-27 16:32:39.000000 django-scim2-0.8.2/CHANGES.txt
+-rw-r--r--   0 paul       (501) staff       (20)     1211 2016-12-13 22:02:05.000000 django-scim2-0.8.2/LICENSE.txt
+-rw-r--r--   0 paul       (501) staff       (20)      196 2016-12-29 07:31:06.000000 django-scim2-0.8.2/MANIFEST.in
+-rw-r--r--   0 paul       (501) staff       (20)     4955 2019-02-27 16:34:02.000000 django-scim2-0.8.2/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     2892 2018-12-22 21:04:19.000000 django-scim2-0.8.2/README.rst
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-27 16:34:02.000000 django-scim2-0.8.2/django_scim/
+-rw-r--r--   0 paul       (501) staff       (20)       22 2019-02-27 16:32:10.000000 django-scim2-0.8.2/django_scim/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)    13251 2019-02-27 15:57:39.000000 django-scim2-0.8.2/django_scim/adapters.py
+-rw-r--r--   0 paul       (501) staff       (20)      804 2017-10-11 18:46:30.000000 django-scim2-0.8.2/django_scim/constants.py
+-rw-r--r--   0 paul       (501) staff       (20)     1098 2018-12-13 23:14:02.000000 django-scim2-0.8.2/django_scim/exceptions.py
+-rw-r--r--   0 paul       (501) staff       (20)    12426 2018-12-13 18:01:06.000000 django-scim2-0.8.2/django_scim/filters.py
+-rw-r--r--   0 paul       (501) staff       (20)     2191 2018-12-13 18:01:06.000000 django-scim2-0.8.2/django_scim/grammars.py
+-rw-r--r--   0 paul       (501) staff       (20)     2601 2019-02-27 16:02:56.000000 django-scim2-0.8.2/django_scim/middleware.py
+-rw-r--r--   0 paul       (501) staff       (20)     7302 2019-02-26 03:40:17.000000 django-scim2-0.8.2/django_scim/models.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-27 16:34:02.000000 django-scim2-0.8.2/django_scim/schemas/
+-rw-r--r--   0 paul       (501) staff       (20)      488 2016-12-13 22:02:05.000000 django-scim2-0.8.2/django_scim/schemas/README.rst
+-rw-r--r--   0 paul       (501) staff       (20)      568 2017-03-09 00:06:19.000000 django-scim2-0.8.2/django_scim/schemas/__init__.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-27 16:34:02.000000 django-scim2-0.8.2/django_scim/schemas/core/
+-rw-r--r--   0 paul       (501) staff       (20)     2051 2016-12-13 22:02:05.000000 django-scim2-0.8.2/django_scim/schemas/core/Group.json
+-rw-r--r--   0 paul       (501) staff       (20)     3215 2016-12-13 22:02:05.000000 django-scim2-0.8.2/django_scim/schemas/core/ResourceType.json
+-rw-r--r--   0 paul       (501) staff       (20)    11445 2016-12-13 22:02:05.000000 django-scim2-0.8.2/django_scim/schemas/core/Schema.json
+-rw-r--r--   0 paul       (501) staff       (20)     6571 2016-12-13 22:02:05.000000 django-scim2-0.8.2/django_scim/schemas/core/ServiceProviderConfig.json
+-rw-r--r--   0 paul       (501) staff       (20)    26634 2016-12-13 22:02:05.000000 django-scim2-0.8.2/django_scim/schemas/core/User.json
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-27 16:34:02.000000 django-scim2-0.8.2/django_scim/schemas/extension/
+-rw-r--r--   0 paul       (501) staff       (20)     3426 2016-12-13 22:02:05.000000 django-scim2-0.8.2/django_scim/schemas/extension/Enterprise-User.json
+-rw-r--r--   0 paul       (501) staff       (20)     4434 2018-12-13 18:55:45.000000 django-scim2-0.8.2/django_scim/settings.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-27 16:34:02.000000 django-scim2-0.8.2/django_scim/tests/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2016-12-13 22:02:05.000000 django-scim2-0.8.2/django_scim/tests/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)      537 2018-12-13 21:54:29.000000 django-scim2-0.8.2/django_scim/tests/hashers.py
+-rw-r--r--   0 paul       (501) staff       (20)     8275 2019-02-26 21:35:11.000000 django-scim2-0.8.2/django_scim/tests/test_adapters.py
+-rw-r--r--   0 paul       (501) staff       (20)     1055 2019-02-13 21:47:15.000000 django-scim2-0.8.2/django_scim/tests/test_grammar.py
+-rw-r--r--   0 paul       (501) staff       (20)     1162 2019-02-27 16:31:19.000000 django-scim2-0.8.2/django_scim/tests/test_middleware.py
+-rw-r--r--   0 paul       (501) staff       (20)     1908 2019-02-26 21:33:11.000000 django-scim2-0.8.2/django_scim/tests/test_models.py
+-rw-r--r--   0 paul       (501) staff       (20)      614 2017-07-25 21:53:37.000000 django-scim2-0.8.2/django_scim/tests/test_utils.py
+-rw-r--r--   0 paul       (501) staff       (20)    33206 2019-02-27 15:57:39.000000 django-scim2-0.8.2/django_scim/tests/test_views.py
+-rw-r--r--   0 paul       (501) staff       (20)      353 2018-06-13 17:08:36.000000 django-scim2-0.8.2/django_scim/tests/urls.py
+-rw-r--r--   0 paul       (501) staff       (20)     1663 2018-12-13 18:01:06.000000 django-scim2-0.8.2/django_scim/urls.py
+-rw-r--r--   0 paul       (501) staff       (20)     3505 2018-12-13 18:55:45.000000 django-scim2-0.8.2/django_scim/utils.py
+-rw-r--r--   0 paul       (501) staff       (20)    14008 2019-02-27 15:57:39.000000 django-scim2-0.8.2/django_scim/views.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2019-02-27 16:34:02.000000 django-scim2-0.8.2/django_scim2.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     4955 2019-02-27 16:34:02.000000 django-scim2-0.8.2/django_scim2.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     1172 2019-02-27 16:34:02.000000 django-scim2-0.8.2/django_scim2.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2019-02-27 16:34:02.000000 django-scim2-0.8.2/django_scim2.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2018-06-12 21:20:24.000000 django-scim2-0.8.2/django_scim2.egg-info/not-zip-safe
+-rw-r--r--   0 paul       (501) staff       (20)       42 2019-02-27 16:34:02.000000 django-scim2-0.8.2/django_scim2.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       12 2019-02-27 16:34:02.000000 django-scim2-0.8.2/django_scim2.egg-info/top_level.txt
+-rw-r--r--   0 paul       (501) staff       (20)       67 2019-02-27 16:34:02.000000 django-scim2-0.8.2/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)     2792 2019-02-27 15:57:39.000000 django-scim2-0.8.2/setup.py
+-rw-r--r--   0 paul       (501) staff       (20)      398 2019-02-11 18:15:56.000000 django-scim2-0.8.2/tox.ini
```

### Comparing `django-scim2-0.8.1/CHANGES.txt` & `django-scim2-0.8.2/CHANGES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 CHANGE LOG
 ==========
+
+0.8.2
+-----
+- Only log during SCIM calls
+
 0.8.1
 -----
 - Fix failing tests
 
 0.8.0
 -----
 - Add basic abstract models for Users and Groups
```

### Comparing `django-scim2-0.8.1/LICENSE.txt` & `django-scim2-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/PKG-INFO` & `django-scim2-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-scim2
-Version: 0.8.1
+Version: 0.8.2
 Summary: A partial implementation of the SCIM 2.0 provider specification for use with Django.
 Home-page: https://github.com/15five/django-scim2
 Author: Paul Logston
 Author-email: paul@15five.com
 Maintainer: Paul Logston
 Maintainer-email: paul@15five.com
 License: MIT
```

### Comparing `django-scim2-0.8.1/README.rst` & `django-scim2-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/adapters.py` & `django-scim2-0.8.2/django_scim/adapters.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/constants.py` & `django-scim2-0.8.2/django_scim/constants.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/exceptions.py` & `django-scim2-0.8.2/django_scim/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/filters.py` & `django-scim2-0.8.2/django_scim/filters.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/grammars.py` & `django-scim2-0.8.2/django_scim/grammars.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/middleware.py` & `django-scim2-0.8.2/django_scim/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         if not hasattr(request, 'user') or request.user.is_anonymous:
             if request.path.startswith(self.reverse_url):
                 response = HttpResponse(status=401)
                 response['WWW-Authenticate'] = scim_settings.WWW_AUTHENTICATE_HEADER
                 return response
 
     def process_response(self, request, response):
-        self.log_call(request, response)
+        if request.path.startswith(self.reverse_url):
+            self.log_call(request, response)
         return response
 
     def get_loggable_request_body(self, request):
         try:
             body = get_loggable_body(request.body.decode(constants.ENCODING))
         except Exception as e:
             body = 'Could not parse request body\n' + str(e)
```

### Comparing `django-scim2-0.8.1/django_scim/models.py` & `django-scim2-0.8.2/django_scim/models.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/schemas/__init__.py` & `django-scim2-0.8.2/django_scim/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/schemas/core/Group.json` & `django-scim2-0.8.2/django_scim/schemas/core/Group.json`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/schemas/core/ResourceType.json` & `django-scim2-0.8.2/django_scim/schemas/core/ResourceType.json`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/schemas/core/Schema.json` & `django-scim2-0.8.2/django_scim/schemas/core/Schema.json`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/schemas/core/ServiceProviderConfig.json` & `django-scim2-0.8.2/django_scim/schemas/core/ServiceProviderConfig.json`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/schemas/core/User.json` & `django-scim2-0.8.2/django_scim/schemas/core/User.json`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/schemas/extension/Enterprise-User.json` & `django-scim2-0.8.2/django_scim/schemas/extension/Enterprise-User.json`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/settings.py` & `django-scim2-0.8.2/django_scim/settings.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/tests/hashers.py` & `django-scim2-0.8.2/django_scim/tests/hashers.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/tests/test_adapters.py` & `django-scim2-0.8.2/django_scim/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/tests/test_grammar.py` & `django-scim2-0.8.2/django_scim/tests/test_grammar.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/tests/test_models.py` & `django-scim2-0.8.2/django_scim/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/tests/test_utils.py` & `django-scim2-0.8.2/django_scim/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/tests/test_views.py` & `django-scim2-0.8.2/django_scim/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/urls.py` & `django-scim2-0.8.2/django_scim/urls.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/utils.py` & `django-scim2-0.8.2/django_scim/utils.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim/views.py` & `django-scim2-0.8.2/django_scim/views.py`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/django_scim2.egg-info/PKG-INFO` & `django-scim2-0.8.2/django_scim2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-scim2
-Version: 0.8.1
+Version: 0.8.2
 Summary: A partial implementation of the SCIM 2.0 provider specification for use with Django.
 Home-page: https://github.com/15five/django-scim2
 Author: Paul Logston
 Author-email: paul@15five.com
 Maintainer: Paul Logston
 Maintainer-email: paul@15five.com
 License: MIT
```

### Comparing `django-scim2-0.8.1/django_scim2.egg-info/SOURCES.txt` & `django-scim2-0.8.2/django_scim2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-scim2-0.8.1/setup.py` & `django-scim2-0.8.2/setup.py`

 * *Files identical despite different names*

