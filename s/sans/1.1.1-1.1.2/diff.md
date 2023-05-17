# Comparing `tmp/sans-1.1.1.tar.gz` & `tmp/sans-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sans-1.1.1.tar", last modified: Wed May 17 20:17:28 2023, max compression
+gzip compressed data, was "sans-1.1.2.tar", last modified: Wed May 17 23:00:13 2023, max compression
```

## Comparing `sans-1.1.1.tar` & `sans-1.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:17:28.221486 sans-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:17:28.213486 sans-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:17:28.213486 sans-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-17 20:17:16.000000 sans-1.1.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-17 20:17:16.000000 sans-1.1.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-17 20:17:16.000000 sans-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-17 20:17:16.000000 sans-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 20:17:16.000000 sans-1.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 20:17:16.000000 sans-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 20:17:28.221486 sans-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-17 20:17:16.000000 sans-1.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:17:28.217486 sans-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-17 20:17:16.000000 sans-1.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-17 20:17:16.000000 sans-1.1.1/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-17 20:17:16.000000 sans-1.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 20:17:16.000000 sans-1.1.1/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 20:17:16.000000 sans-1.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-17 20:17:16.000000 sans-1.1.1/docs/limiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 20:17:16.000000 sans-1.1.1/docs/lock.rst
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-17 20:17:16.000000 sans-1.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 20:17:16.000000 sans-1.1.1/docs/response.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-17 20:17:16.000000 sans-1.1.1/docs/url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 20:17:16.000000 sans-1.1.1/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-17 20:17:16.000000 sans-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-17 20:17:16.000000 sans-1.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:17:28.221486 sans-1.1.1/sans/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-17 20:17:16.000000 sans-1.1.1/sans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-17 20:17:16.000000 sans-1.1.1/sans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-17 20:17:16.000000 sans-1.1.1/sans/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-17 20:17:16.000000 sans-1.1.1/sans/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-17 20:17:16.000000 sans-1.1.1/sans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-05-17 20:17:16.000000 sans-1.1.1/sans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-17 20:17:16.000000 sans-1.1.1/sans/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-17 20:17:16.000000 sans-1.1.1/sans/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-17 20:17:16.000000 sans-1.1.1/sans/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-17 20:17:16.000000 sans-1.1.1/sans/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:17:16.000000 sans-1.1.1/sans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-17 20:17:16.000000 sans-1.1.1/sans/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-17 20:17:16.000000 sans-1.1.1/sans/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-17 20:17:16.000000 sans-1.1.1/sans/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:17:28.221486 sans-1.1.1/sans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 20:17:28.000000 sans-1.1.1/sans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-17 20:17:28.000000 sans-1.1.1/sans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:17:28.000000 sans-1.1.1/sans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 20:17:28.000000 sans-1.1.1/sans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 20:17:28.000000 sans-1.1.1/sans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 20:17:28.000000 sans-1.1.1/sans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:17:28.221486 sans-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-17 20:17:16.000000 sans-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:00:13.285001 sans-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:00:13.277001 sans-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:00:13.281001 sans-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-17 23:00:01.000000 sans-1.1.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-17 23:00:01.000000 sans-1.1.2/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-17 23:00:01.000000 sans-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-17 23:00:01.000000 sans-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 23:00:01.000000 sans-1.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 23:00:01.000000 sans-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 23:00:13.285001 sans-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-17 23:00:01.000000 sans-1.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:00:13.281001 sans-1.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-17 23:00:01.000000 sans-1.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-17 23:00:01.000000 sans-1.1.2/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-17 23:00:01.000000 sans-1.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 23:00:01.000000 sans-1.1.2/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 23:00:01.000000 sans-1.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-17 23:00:01.000000 sans-1.1.2/docs/limiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 23:00:01.000000 sans-1.1.2/docs/lock.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-17 23:00:01.000000 sans-1.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 23:00:01.000000 sans-1.1.2/docs/response.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-17 23:00:01.000000 sans-1.1.2/docs/url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 23:00:01.000000 sans-1.1.2/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-17 23:00:01.000000 sans-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-17 23:00:01.000000 sans-1.1.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:00:13.285001 sans-1.1.2/sans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-17 23:00:01.000000 sans-1.1.2/sans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-17 23:00:01.000000 sans-1.1.2/sans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-17 23:00:01.000000 sans-1.1.2/sans/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-17 23:00:01.000000 sans-1.1.2/sans/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-17 23:00:01.000000 sans-1.1.2/sans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-05-17 23:00:01.000000 sans-1.1.2/sans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-17 23:00:01.000000 sans-1.1.2/sans/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-17 23:00:01.000000 sans-1.1.2/sans/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-17 23:00:01.000000 sans-1.1.2/sans/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-17 23:00:01.000000 sans-1.1.2/sans/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 23:00:01.000000 sans-1.1.2/sans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-17 23:00:01.000000 sans-1.1.2/sans/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-17 23:00:01.000000 sans-1.1.2/sans/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-17 23:00:01.000000 sans-1.1.2/sans/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:00:13.285001 sans-1.1.2/sans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 23:00:13.000000 sans-1.1.2/sans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-17 23:00:13.000000 sans-1.1.2/sans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 23:00:13.000000 sans-1.1.2/sans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 23:00:13.000000 sans-1.1.2/sans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 23:00:13.000000 sans-1.1.2/sans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 23:00:13.000000 sans-1.1.2/sans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 23:00:13.285001 sans-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-17 23:00:01.000000 sans-1.1.2/setup.py
```

### Comparing `sans-1.1.1/.github/workflows/codeql-analysis.yml` & `sans-1.1.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/.github/workflows/pythonpublish.yml` & `sans-1.1.2/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/.gitignore` & `sans-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/.pre-commit-config.yaml` & `sans-1.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/LICENSE` & `sans-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/PKG-INFO` & `sans-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.1.1
+Version: 1.1.2
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sans-1.1.1/README.rst` & `sans-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/docs/Makefile` & `sans-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/docs/conf.py` & `sans-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/docs/make.bat` & `sans-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/pyproject.toml` & `sans-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/__init__.py` & `sans-1.1.2/sans/__init__.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/__main__.py` & `sans-1.1.2/sans/__main__.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/_state.py` & `sans-1.1.2/sans/_state.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/auth.py` & `sans-1.1.2/sans/auth.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/client.py` & `sans-1.1.2/sans/client.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/client.pyi` & `sans-1.1.2/sans/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,17 @@
 )
 
 from .limiter import RateLimiter
 from .response import Response
 
 __all__ = [
     "Client",
+    "ClientType",
     "AsyncClient",
+    "AsyncClientType",
     "delete",
     "get",
     "head",
     "options",
     "patch",
     "post",
     "put",
@@ -91,15 +93,15 @@
         content: RequestContent = ...,
         data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     def send(
         self,
@@ -111,15 +113,15 @@
     ) -> Response: ...
     @overload
     def send(
         self,
         request: httpx.Request,
         *,
         stream: bool = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
     ) -> httpx.Response: ...
     @overload
     def get(
         self,
         url: URLTypes,
         *,
@@ -135,15 +137,15 @@
     def get(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     def options(
         self,
@@ -161,15 +163,15 @@
     def options(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     def head(
         self,
@@ -187,15 +189,15 @@
     def head(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     def post(
         self,
@@ -221,15 +223,15 @@
         content: RequestContent = ...,
         data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     def put(
         self,
@@ -255,15 +257,15 @@
         content: RequestContent = ...,
         data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     def patch(
         self,
@@ -289,15 +291,15 @@
         content: RequestContent = ...,
         data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     def delete(
         self,
@@ -315,15 +317,15 @@
     def delete(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     def stream(
         self,
@@ -351,15 +353,15 @@
         content: RequestContent = ...,
         data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> ContextManager[httpx.Response]: ...
 
 class _AsyncClientType(_ClientMixin, httpx.AsyncClient):
     @overload
@@ -389,15 +391,15 @@
         content: RequestContent = ...,
         data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     async def send(
         self,
@@ -409,15 +411,15 @@
     ) -> Response: ...
     @overload
     async def send(
         self,
         request: httpx.Request,
         *,
         stream: bool = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
     ) -> httpx.Response: ...
     @overload
     async def get(
         self,
         url: URLTypes,
         *,
@@ -433,15 +435,15 @@
     async def get(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     async def options(
         self,
@@ -459,15 +461,15 @@
     async def options(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     async def head(
         self,
@@ -485,15 +487,15 @@
     async def head(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     async def post(
         self,
@@ -519,15 +521,15 @@
         content: RequestContent = ...,
         data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     async def put(
         self,
@@ -553,15 +555,15 @@
         content: RequestContent = ...,
         data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     async def patch(
         self,
@@ -587,15 +589,15 @@
         content: RequestContent = ...,
         data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     async def delete(
         self,
@@ -613,15 +615,15 @@
     async def delete(
         self,
         url: URLTypes,
         *,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> httpx.Response: ...
     @overload
     def stream(
         self,
@@ -649,15 +651,15 @@
         content: RequestContent = ...,
         data: RequestData = ...,
         files: RequestFiles = ...,
         json: Any = ...,
         params: QueryParamTypes = ...,
         headers: HeaderTypes = ...,
         cookies: CookieTypes = ...,
-        auth: AuthTypes,
+        auth: AuthTypes | None,
         follow_redirects: bool = ...,
         timeout: TimeoutTypes = ...,
         extensions: dict[Any, Any] = ...,
     ) -> AsyncContextManager[httpx.Response]: ...
 
 ClientType = NewType("ClientType", _ClientType)
 AsyncClientType = NewType("AsyncClientType", _AsyncClientType)
@@ -684,15 +686,15 @@
     transport: httpx.BaseTransport = ...,
     app: Callable[..., Any] = ...,
     trust_env: bool = ...,
 ) -> ClientType: ...
 @overload
 def Client(
     *,
-    auth: AuthTypes,
+    auth: AuthTypes | None,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     http1: bool = ...,
     http2: bool = ...,
@@ -730,15 +732,15 @@
     transport: httpx.BaseTransport = ...,
     app: Callable[..., Any] = ...,
     trust_env: bool = ...,
 ) -> AsyncClientType: ...
 @overload
 def AsyncClient(
     *,
-    auth: AuthTypes,
+    auth: AuthTypes | None,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     http1: bool = ...,
     http2: bool = ...,
@@ -782,15 +784,15 @@
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
     data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes,
+    auth: AuthTypes | None,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
 ) -> httpx.Response: ...
@@ -822,15 +824,15 @@
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
     data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes,
+    auth: AuthTypes | None,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
 ) -> ContextManager[httpx.Response]: ...
@@ -852,15 +854,15 @@
 @overload
 def get(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes,
+    auth: AuthTypes | None,
     proxies: ProxiesTypes = ...,
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> httpx.Response: ...
@@ -882,15 +884,15 @@
 @overload
 def options(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes,
+    auth: AuthTypes | None,
     proxies: ProxiesTypes = ...,
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> httpx.Response: ...
@@ -912,15 +914,15 @@
 @overload
 def head(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes,
+    auth: AuthTypes | None,
     proxies: ProxiesTypes = ...,
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> httpx.Response: ...
@@ -950,15 +952,15 @@
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
     data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes,
+    auth: AuthTypes | None,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
 ) -> httpx.Response: ...
@@ -988,15 +990,15 @@
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
     data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes,
+    auth: AuthTypes | None,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
 ) -> httpx.Response: ...
@@ -1026,15 +1028,15 @@
     params: QueryParamTypes = ...,
     content: RequestContent = ...,
     data: RequestData = ...,
     files: RequestFiles = ...,
     json: Any = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes,
+    auth: AuthTypes | None,
     proxies: ProxiesTypes = ...,
     timeout: TimeoutTypes = ...,
     follow_redirects: bool = ...,
     verify: VerifyTypes = ...,
     cert: CertTypes = ...,
     trust_env: bool = ...,
 ) -> httpx.Response: ...
@@ -1056,15 +1058,15 @@
 @overload
 def delete(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes,
+    auth: AuthTypes | None,
     proxies: ProxiesTypes = ...,
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> httpx.Response: ...
```

### Comparing `sans-1.1.1/sans/decoder.py` & `sans-1.1.2/sans/decoder.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/errors.py` & `sans-1.1.2/sans/errors.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/limiter.py` & `sans-1.1.2/sans/limiter.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/lock.py` & `sans-1.1.2/sans/lock.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/response.py` & `sans-1.1.2/sans/response.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/url.py` & `sans-1.1.2/sans/url.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans/utils.py` & `sans-1.1.2/sans/utils.py`

 * *Files identical despite different names*

### Comparing `sans-1.1.1/sans.egg-info/PKG-INFO` & `sans-1.1.2/sans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.1.1
+Version: 1.1.2
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sans-1.1.1/sans.egg-info/SOURCES.txt` & `sans-1.1.2/sans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

