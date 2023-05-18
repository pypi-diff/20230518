# Comparing `tmp/fresco-3.3.0.tar.gz` & `tmp/fresco-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fresco-3.3.0.tar", last modified: Tue May  2 14:38:24 2023, max compression
+gzip compressed data, was "fresco-3.3.1.tar", last modified: Thu May 18 12:04:33 2023, max compression
```

## Comparing `fresco-3.3.0.tar` & `fresco-3.3.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.318645 fresco-3.3.0/
--rw-r--r--   0 oliver    (1001) wheel        (0)    20513 2023-05-02 14:35:11.000000 fresco-3.3.0/CHANGELOG.rst
--rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-05-02 14:35:09.000000 fresco-3.3.0/LICENSE.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)       50 2023-05-02 14:35:09.000000 fresco-3.3.0/MANIFEST.in
--rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-05-02 14:38:24.318758 fresco-3.3.0/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)      822 2023-05-02 14:35:09.000000 fresco-3.3.0/README.rst
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.310052 fresco-3.3.0/fresco/
--rw-r--r--   0 oliver    (1001) wheel        (0)     3520 2023-05-02 14:38:20.000000 fresco-3.3.0/fresco/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7055 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/cookie.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    26551 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/core.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3232 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/decorators.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4410 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4173 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/middleware.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    13362 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/multidict.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    13614 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/options.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    27071 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/request.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3504 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/requestcontext.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    37078 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/response.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10176 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/routeargs.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    57738 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/routing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2513 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/static.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    11025 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/subrequests.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.314384 fresco-3.3.0/fresco/tests/
--rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1871 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/fixtures.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2171 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_cookie.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    34019 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_core.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1480 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_decorators.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      973 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3137 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_middleware.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7565 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_multidict.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10868 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_options.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    16389 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_request.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3115 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_requestcontext.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8934 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_response.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8162 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_routeargs.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    36812 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_routing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4686 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_static.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7909 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/test_subrequests.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.315889 fresco-3.3.0/fresco/tests/util/
--rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10570 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/form_data.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1117 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/test_common.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10803 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/test_http.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1492 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/test_security.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7643 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/test_urls.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3038 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/tests/util/test_wsgi.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      106 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/types.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      347 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/typing.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.318452 fresco-3.3.0/fresco/util/
--rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1609 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/cache.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1258 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/common.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     5484 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/contentencodings.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1383 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/file.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    22175 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/http.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1289 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/io.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      370 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/object.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1058 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/security.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2309 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/textproc.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     9195 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/urls.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    12970 2023-05-02 14:35:09.000000 fresco-3.3.0/fresco/util/wsgi.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-02 14:38:24.310894 fresco-3.3.0/fresco.egg-info/
--rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-05-02 14:38:24.000000 fresco-3.3.0/fresco.egg-info/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)     1476 2023-05-02 14:38:24.000000 fresco-3.3.0/fresco.egg-info/SOURCES.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-05-02 14:38:24.000000 fresco-3.3.0/fresco.egg-info/dependency_links.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-05-02 14:38:24.000000 fresco-3.3.0/fresco.egg-info/top_level.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)      795 2023-05-02 14:38:24.319366 fresco-3.3.0/setup.cfg
--rw-r--r--   0 oliver    (1001) wheel        (0)      634 2023-05-02 14:35:09.000000 fresco-3.3.0/setup.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.167537 fresco-3.3.1/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    20745 2023-05-18 12:01:48.000000 fresco-3.3.1/CHANGELOG.rst
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-05-18 12:01:48.000000 fresco-3.3.1/LICENSE.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)       50 2023-05-18 12:01:48.000000 fresco-3.3.1/MANIFEST.in
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-05-18 12:04:33.167646 fresco-3.3.1/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)      822 2023-05-18 12:01:48.000000 fresco-3.3.1/README.rst
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.159011 fresco-3.3.1/fresco/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3520 2023-05-18 12:04:31.000000 fresco-3.3.1/fresco/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7055 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/cookie.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    26615 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/core.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3232 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/decorators.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4410 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4173 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/middleware.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    13362 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/multidict.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    13614 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/options.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    27071 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/request.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3504 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/requestcontext.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    37078 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/response.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10176 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/routeargs.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    58670 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/routing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2513 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/static.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11081 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/subrequests.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.163318 fresco-3.3.1/fresco/tests/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1871 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/fixtures.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2171 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_cookie.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    34019 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_core.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1480 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_decorators.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      973 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3137 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_middleware.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7565 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_multidict.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10868 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_options.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    16389 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_request.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3115 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_requestcontext.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     8934 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_response.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     8162 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_routeargs.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    37207 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_routing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4686 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_static.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7909 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_subrequests.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.164807 fresco-3.3.1/fresco/tests/util/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10570 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/form_data.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1117 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/test_common.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10803 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/test_http.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1492 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/test_security.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7643 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/test_urls.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3038 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/test_wsgi.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      106 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/types.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      347 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/typing.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.167353 fresco-3.3.1/fresco/util/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1609 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/cache.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1258 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/common.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     5484 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/contentencodings.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1383 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/file.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    22175 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/http.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1289 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/io.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      370 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/object.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1058 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/security.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2309 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/textproc.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9195 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/urls.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    12970 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/wsgi.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.159850 fresco-3.3.1/fresco.egg-info/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-05-18 12:04:32.000000 fresco-3.3.1/fresco.egg-info/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1476 2023-05-18 12:04:32.000000 fresco-3.3.1/fresco.egg-info/SOURCES.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-05-18 12:04:32.000000 fresco-3.3.1/fresco.egg-info/dependency_links.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-05-18 12:04:32.000000 fresco-3.3.1/fresco.egg-info/top_level.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)      795 2023-05-18 12:04:33.168250 fresco-3.3.1/setup.cfg
+-rw-r--r--   0 oliver    (1001) wheel        (0)      634 2023-05-18 12:01:48.000000 fresco-3.3.1/setup.py
```

### Comparing `fresco-3.3.0/CHANGELOG.rst` & `fresco-3.3.1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 Changelog
 =========
 
-3.3.0 (released 2023-05-02)
+3.3.1 (released 2023-05-18)
 ---------------------------
 
+- The ``route_wsgi`` and ``route_all`` methods now only match at a
+  path separator boundary (``'/'``).
+- Bugfix: subrequest now works with views routed via ``RRoute`` (and so expect
+  an initial ``request`` argument)
+
+3.3.0
+-----
+
 - Options: fresco.options.Options can now take a list of paths as its first argument
 - Options: tags can now be specified with environment variable substitutions
   (eg "{FOO}" would load files tagged with the current value of the 'FOO'
   environment variable)
 - Options: add ``fresco.options.list_from_str`` and ``fresco.options.dict_from_options``
 
 3.2.0 (released 2023-04-16)
```

### Comparing `fresco-3.3.0/LICENSE.txt` & `fresco-3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/PKG-INFO` & `fresco-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fresco
-Version: 3.3.0
+Version: 3.3.1
 Summary: A Web/WSGI micro-framework
 Home-page: https://ollycope.com/software/fresco/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi web www framework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fresco-3.3.0/README.rst` & `fresco-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/__init__.py` & `fresco-3.3.1/fresco/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
-__version__ = "3.3.0"
+__version__ = "3.3.1"
 
 DEFAULT_CHARSET = "UTF-8"
 
 __all__ = [
     "Request",
     "currentrequest",
     "context",
```

### Comparing `fresco-3.3.0/fresco/cookie.py` & `fresco-3.3.1/fresco/cookie.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/core.py` & `fresco-3.3.1/fresco/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         # Is the URL matched by another HTTP method?
         methods = self.get_methods(request, path)
         if methods:
             return Response.method_not_allowed(methods)
 
         # Is the URL just missing a trailing '/'?
         if not path or path[-1] != "/":
-            for _ in self.get_methods(request, path + "/"):
+            if self.get_methods(request, path + "/"):
                 return Response.unrestricted_redirect_permanent(path + "/")
 
         return Response.not_found()
 
     def view(self, request: t.Optional[Request] = None) -> Response:
         request = request or context.request
         try:
@@ -283,15 +283,17 @@
 
         if "400" <= response.status <= "599":
             if self.process_http_error_response_handlers:
                 response = self.handle_http_error_response(request, response)
 
         return response
 
-    def handle_http_error_response(self, request, response):
+    def handle_http_error_response(
+        self, request: Request, response: Response
+    ) -> Response:
         """
         Call any process_http_error_response handlers and return the
         (potentially modified) response object.
         """
         for status, f in self.process_http_error_response_handlers:
             try:
                 if status is not None and status != response.status_code:
@@ -299,16 +301,16 @@
                 r = f(request, response)
                 if r is not None:
                     response = r
             except Exception:
                 self.log_exception(request)
         return response
 
-    def get_methods(self, request, path):
-        """\
+    def get_methods(self, request: Request, path: str) -> Set[str]:
+        """
         Return the HTTP methods valid in routes to the given path
         """
         methods: Set[str] = set()
         for traversal in self.get_route_traversals(path, None):
             route = traversal.route
             if route.predicate and not route.predicate(request):
                 continue
```

### Comparing `fresco-3.3.0/fresco/decorators.py` & `fresco-3.3.1/fresco/decorators.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/exceptions.py` & `fresco-3.3.1/fresco/exceptions.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/middleware.py` & `fresco-3.3.1/fresco/middleware.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/multidict.py` & `fresco-3.3.1/fresco/multidict.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/options.py` & `fresco-3.3.1/fresco/options.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/request.py` & `fresco-3.3.1/fresco/request.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/requestcontext.py` & `fresco-3.3.1/fresco/requestcontext.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/response.py` & `fresco-3.3.1/fresco/response.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/routeargs.py` & `fresco-3.3.1/fresco/routeargs.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/routing.py` & `fresco-3.3.1/fresco/routing.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,23 +366,23 @@
     ``str`` object.
     """
 
     pattern = r".+"
 
 
 class MatchAllURLsPattern(Pattern):
-    """\
-    A pattern matcher that matches all URLs starting with the given prefix. No
-    arguments are parsed from the URL.
+    """
+    A pattern matcher that matches all paths starting with the given prefix.
+    No arguments are parsed from the URL.
     """
 
     def __init__(self, path):
         self.path = path
 
-    def match(self, path):
+    def match(self, path: str) -> t.Optional[PathMatch]:
         if path.startswith(self.path):
             return PathMatch(self.path, path[len(self.path) :], (), {})
         return None
 
     def pathfor(self, *args, **kwargs):
         assert (
             not args and not kwargs
@@ -396,14 +396,40 @@
     def add_prefix(self, prefix):
         return self.__class__(join_path(prefix, self.path))
 
     def __str__(self):
         return "%s*" % (self.path,)
 
 
+class PrefixPattern(MatchAllURLsPattern):
+    """
+    A pattern matcher that matches the given prefix. The prefix will only be
+    matched at a path separator boundary.
+
+    ``PrefixPattern('/foo')`` will match the paths ``/foo`` and ``/foo/bar``,
+    but not ``/foobar``.
+
+    No arguments are parsed from the URL.
+    """
+
+    def __init__(self, path):
+        super().__init__(path)
+        if path[-1] == "/":
+            self.path_with_sep = path
+        else:
+            self.path_with_sep = f"{self.path}/"
+
+    def match(self, path: str) -> t.Optional[PathMatch]:
+        prefix = path[: len(self.path_with_sep)]
+
+        if prefix == self.path or prefix == self.path_with_sep:
+            return PathMatch(self.path, path[len(self.path) :], (), {})
+        return None
+
+
 class ExtensiblePattern(Pattern):
     """\
     An extensible URL pattern matcher.
 
     Synopsis::
 
         >>> from pprint import pprint
@@ -543,18 +569,18 @@
             ((1, 2, 'buckle my shoe'), {})
             >>> ep.parseargs("3, four='knock on the door'")
             ((3,), {'four': 'knock on the door'})
 
         """
         return eval("(lambda *args, **kwargs: (args, kwargs))(%s)" % argstr)
 
-    def match(self, path):
+    def match(self, path) -> t.Optional[PathMatch]:
         """
-        Test ``path`` and return a tuple of parsed ``(args, kwargs)``, or
-        ``None`` if there was no match.
+        Test ``path`` and return a PathMatch object or ``None`` if there was no
+        match.
         """
         mo = self.regex_match(path)
         if mo is None:
             return None
         groups = mo.groups()
         assert len(groups) == len(self.args), (
             "Number of regex groups does not match expected count. "
@@ -1354,21 +1380,26 @@
                     if isinstance(route_or_rnf, RouteNotFound):
                         raise route_or_rnf
                     return route_or_rnf
                 else:
                     exc = self.__routed_views__[viewspec] = RouteNotFound(viewspec)
                     raise exc
 
-    def _get_routes(self, key):
+    def _get_routes(
+        self, key: Tuple[t.Optional[str], str]
+    ) -> t.Sequence[t.Tuple[Route, t.Optional[PathMatch]]]:
         method, path = key
         routes = ((r, r.match(path, method)) for r in self.__routes__)
         return [(r, t) for (r, t) in routes if t is not None]
 
     def get_route_traversals(
-        self, path: str, method: Optional[str], request: Optional[Request] = None
+        self,
+        path: str,
+        method: Optional[str],
+        request: Optional[Request] = None,
     ) -> t.Iterator[RouteTraversal]:
         """
         Generate RouteTraversals for routes matching the given path and
         method::
 
             for rt in routecollection.get_route_traversals('/foo/bar', GET):
                 print("Route is", rt.route)
@@ -1600,15 +1631,15 @@
     ):
         """
         Expose a view for all URLs starting with ``path``.
 
         :param path: the path prefix at which the view will be routed
         """
         return self.route(
-            MatchAllURLsPattern(path),
+            PrefixPattern(path),
             methods,
             view,
             route_class=route_class,
             *args,
             **kwargs,
         )
```

### Comparing `fresco-3.3.0/fresco/static.py` & `fresco-3.3.1/fresco/static.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/subrequests.py` & `fresco-3.3.1/fresco/subrequests.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,15 @@
     Return the args/kwargs required to pass to the view callable for ``route``.
     """
     mutable_args = list(args)
     mutable_kwargs = kwargs.copy()
     route_kwargs = {}
     route_args = list(
         chain(
+            [request] if route.provide_request else [],
             ((a(request) if isinstance(a, RouteArg) else a) for a in route.view_args),
             (
                 mutable_args.pop(0)
                 for a in route.pattern.segments
                 if a.converter and not a.name
             ),
         )
```

### Comparing `fresco-3.3.0/fresco/tests/fixtures.py` & `fresco-3.3.1/fresco/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_cookie.py` & `fresco-3.3.1/fresco/tests/test_cookie.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_core.py` & `fresco-3.3.1/fresco/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_decorators.py` & `fresco-3.3.1/fresco/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_exceptions.py` & `fresco-3.3.1/fresco/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_middleware.py` & `fresco-3.3.1/fresco/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_multidict.py` & `fresco-3.3.1/fresco/tests/test_multidict.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_options.py` & `fresco-3.3.1/fresco/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_request.py` & `fresco-3.3.1/fresco/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_requestcontext.py` & `fresco-3.3.1/fresco/tests/test_requestcontext.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_response.py` & `fresco-3.3.1/fresco/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_routeargs.py` & `fresco-3.3.1/fresco/tests/test_routeargs.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_routing.py` & `fresco-3.3.1/fresco/tests/test_routing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1088,7 +1088,21 @@
             list(rc.get_route_traversals("/eggs/x", GET))
 
         with pytest.raises(CustomException):
             list(rc.get_route_traversals("/eggs/x", GET))
 
         # Check a subsequent call to get_routes doesn't hang onto the exception
         list(rc.get_route_traversals("/bacon", GET))
+
+
+class TestRouteAll:
+
+    def test_route_all_matches_on_separator(self):
+        def view():
+            return Response()
+
+        app = FrescoApp()
+        app.route_all("/x", GET, view)
+
+        assert len(list(app.get_route_traversals("/x", GET))) == 1
+        assert len(list(app.get_route_traversals("/x/y", GET))) == 1
+        assert len(list(app.get_route_traversals("/xy", GET))) == 0
```

### Comparing `fresco-3.3.0/fresco/tests/test_static.py` & `fresco-3.3.1/fresco/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/test_subrequests.py` & `fresco-3.3.1/fresco/tests/test_subrequests.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/util/form_data.py` & `fresco-3.3.1/fresco/tests/util/form_data.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/util/test_common.py` & `fresco-3.3.1/fresco/tests/util/test_common.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/util/test_http.py` & `fresco-3.3.1/fresco/tests/util/test_http.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/util/test_security.py` & `fresco-3.3.1/fresco/tests/util/test_security.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/util/test_urls.py` & `fresco-3.3.1/fresco/tests/util/test_urls.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/tests/util/test_wsgi.py` & `fresco-3.3.1/fresco/tests/util/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/util/cache.py` & `fresco-3.3.1/fresco/util/cache.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/util/common.py` & `fresco-3.3.1/fresco/util/common.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/util/contentencodings.py` & `fresco-3.3.1/fresco/util/contentencodings.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/util/file.py` & `fresco-3.3.1/fresco/util/file.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/util/http.py` & `fresco-3.3.1/fresco/util/http.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/util/io.py` & `fresco-3.3.1/fresco/util/io.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/util/security.py` & `fresco-3.3.1/fresco/util/security.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/util/textproc.py` & `fresco-3.3.1/fresco/util/textproc.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/util/urls.py` & `fresco-3.3.1/fresco/util/urls.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco/util/wsgi.py` & `fresco-3.3.1/fresco/util/wsgi.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/fresco.egg-info/PKG-INFO` & `fresco-3.3.1/fresco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fresco
-Version: 3.3.0
+Version: 3.3.1
 Summary: A Web/WSGI micro-framework
 Home-page: https://ollycope.com/software/fresco/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi web www framework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fresco-3.3.0/fresco.egg-info/SOURCES.txt` & `fresco-3.3.1/fresco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/setup.cfg` & `fresco-3.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fresco-3.3.0/setup.py` & `fresco-3.3.1/setup.py`

 * *Files identical despite different names*

