# Comparing `tmp/django-opensearch-dsl-0.5.0.tar.gz` & `tmp/django-opensearch-dsl-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-opensearch-dsl-0.5.0.tar", last modified: Sun Nov 20 15:58:23 2022, max compression
+gzip compressed data, was "django-opensearch-dsl-0.5.1.tar", last modified: Thu May 18 00:08:17 2023, max compression
```

## Comparing `django-opensearch-dsl-0.5.0.tar` & `django-opensearch-dsl-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 15:58:23.324458 django-opensearch-dsl-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3870 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12106 2022-11-20 15:58:23.328458 django-opensearch-dsl-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4825 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 15:58:23.324458 django-opensearch-dsl-0.5.0/django_opensearch_dsl/
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     9227 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/documents.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8179 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/indices.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 15:58:23.324458 django-opensearch-dsl-0.5.0/django_opensearch_dsl/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 15:58:23.324458 django-opensearch-dsl-0.5.0/django_opensearch_dsl/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14631 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/management/commands/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/management/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/management/types.py
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6591 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/registries.py
--rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/search.py
--rw-r--r--   0 runner    (1001) docker     (121)     3183 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 15:58:23.324458 django-opensearch-dsl-0.5.0/django_opensearch_dsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12106 2022-11-20 15:58:23.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-11-20 15:58:23.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-20 15:58:23.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-20 15:58:23.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-20 15:58:23.000000 django-opensearch-dsl-0.5.0/django_opensearch_dsl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 15:58:23.324458 django-opensearch-dsl-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6211 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-11-20 15:58:23.328458 django-opensearch-dsl-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1608 2022-11-20 15:58:22.000000 django-opensearch-dsl-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:08:17.229260 django-opensearch-dsl-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-05-18 00:08:17.229260 django-opensearch-dsl-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:08:17.225260 django-opensearch-dsl-0.5.1/django_opensearch_dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/indices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:08:17.229260 django-opensearch-dsl-0.5.1/django_opensearch_dsl/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:08:17.229260 django-opensearch-dsl-0.5.1/django_opensearch_dsl/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14631 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/management/commands/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/management/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/management/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:08:17.229260 django-opensearch-dsl-0.5.1/django_opensearch_dsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-05-18 00:08:17.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-18 00:08:17.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 00:08:17.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 00:08:17.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 00:08:17.000000 django-opensearch-dsl-0.5.1/django_opensearch_dsl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 00:08:17.229260 django-opensearch-dsl-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-18 00:08:17.229260 django-opensearch-dsl-0.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1609 2023-05-18 00:08:16.000000 django-opensearch-dsl-0.5.1/setup.py
```

### Comparing `django-opensearch-dsl-0.5.0/CONTRIBUTING.md` & `django-opensearch-dsl-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.5.0/LICENSE` & `django-opensearch-dsl-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.5.0/PKG-INFO` & `django-opensearch-dsl-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-opensearch-dsl
-Version: 0.5.0
-Summary: Wrapper around opensearch-dsl-py for django models
+Version: 0.5.1
+Summary: Wrapper around opensearch-py for django models
 Home-page: https://github.com/qcoumes/django-opensearch-dsl
 Author: Quentin Coumes (Codoc)
 Author-email: coumes.quentin@gmail.com
 License: Apache Software License 2.0
-Keywords: django elasticsearch elasticsearch-dsl opensearch opensearch-dsl
+Keywords: django elasticsearch elasticsearch-dsl opensearch opensearch-dsl opensearch-py
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -33,37 +33,37 @@
 [![Python 3.7+](https://img.shields.io/badge/Python-3.6+-brightgreen.svg)](#)
 [![Django 3.2+](https://img.shields.io/badge/Django-2.1+-brightgreen.svg)](#)
 [![License Apache 2](https://img.shields.io/badge/license-Apache%202-brightgreen.svg)](https://github.com/Codoc-os/django-opensearch-dsl/blob/master/LICENSE)
 [![codecov](https://codecov.io/gh/Codoc-os/django-opensearch-dsl/branch/master/graph/badge.svg)](https://codecov.io/gh/Codoc-os/django-opensearch-dsl)
 [![CodeFactor](https://www.codefactor.io/repository/github/Codoc-os/django-opensearch-dsl/badge)](https://www.codefactor.io/repository/github/Codoc-os/django-opensearch-dsl)
 
 **Django Opensearch DSL** is a package that allows the indexing of Django models in opensearch. It is built as a thin
-wrapper around [`opensearch-dsl-py`](https://github.com/opensearch-project/opensearch-dsl-py)
-so you can use all the features developed by the `opensearch-dsl` team.
+wrapper around [`opensearch-py`](https://github.com/opensearch-project/opensearch-py)
+so you can use all the features developed by the `opensearch-py` team.
 
 You can view the full documentation
 at [https://django-opensearch-dsl.readthedocs.io](https://django-opensearch-dsl.readthedocs.io/en/latest/).
 
 ## Features
 
-- Based on [`opensearch-dsl-py`](https://github.com/opensearch-project/opensearch-dsl-py) so you can make queries with
+- Based on [`opensearch-py`](https://github.com/opensearch-project/opensearch-py) so you can make queries with
   the [`Search`](https://elasticsearch-dsl.readthedocs.io/en/latest/search_dsl.html#the-search-object)
   object.
 - Management commands for creating, deleting, and populating indices and documents.
 - Opensearch auto mapping from Django models fields.
 - Complex field type support (`ObjectField`, `NestedField`).
 - Index fast using `parallel` indexing.
 
 ## Requirements
 
 `django-opensearch-dsl` only support the supported version of each dependency (mainstream & lts).
 
 * `Python>=3.7`
 * `django>=3.2`
-* `opensearch-dsl>=1.0.0, <3.0.0`
+* `opensearch-py>=1.0.0, <3.0.0`
 * `python-dateutil~=2.8.2`
 
 ## Installation and Configuration
 
 The easiest way to install `django-opensearch-dsl` is through `pip`:
 
 * `pip install django-opensearch-dsl`
@@ -84,15 +84,15 @@
         'http_auth': ("admin", "password"),
         'timeout': 120,
     },
 }
 ```
 
 `OPENSEARCH_DSL` is then passed
-to [`opensearch_dsl_py.connections.configure`](http://elasticsearch-dsl.readthedocs.io/en/stable/configuration.html#multiple-clusters)
+to [`opensearchpy.connection.connections.configure`](http://elasticsearch-dsl.readthedocs.io/en/stable/configuration.html#multiple-clusters)
 .
 
 ## Create Document Classes
 
 To index instances of the following model :
 
 ```python
@@ -147,14 +147,22 @@
         # Paginate the django queryset used to populate the index with the specified size
         # This per-Document setting overrides settings.OPENSEARCH_DSL_QUERYSET_PAGINATION.
         queryset_pagination = 5000
 ```
 
 # Changelog
 
+### 0.5.1 (2023-05-18)
+
+* Change references from `opensearch-dsl-py` to `opensearch-py`.  
+  This follow the deprecation notice on the
+  [`opensearch-dsl-py`](https://github.com/opensearch-project/opensearch-dsl-py) project. Its features are now directly
+  included in `opensearch-py`.  
+  ([#33](https://github.com/Codoc-os/django-opensearch-dsl/issues/33), Contributed by [Jacob Kausler](https://github.com/jakekausler)).
+
 ## 0.5.0 (2022-11-19)
 
 * `get_indexing_queryset()` now order unordered QuerySet by their PK.
   ([#29](https://github.com/Codoc-os/django-opensearch-dsl/issues/29), Contributed by [Cédric Raud](https://github.com/cedricraud)).
 * `keep_order` argument of `django_opensearch_dsl.search.Search.to_queryset` now default to `True`
   to be in line with the documentation ([#27](https://github.com/Codoc-os/django-opensearch-dsl/issues/27)).
```

### Comparing `django-opensearch-dsl-0.5.0/README.md` & `django-opensearch-dsl-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,37 +7,37 @@
 [![Python 3.7+](https://img.shields.io/badge/Python-3.6+-brightgreen.svg)](#)
 [![Django 3.2+](https://img.shields.io/badge/Django-2.1+-brightgreen.svg)](#)
 [![License Apache 2](https://img.shields.io/badge/license-Apache%202-brightgreen.svg)](https://github.com/Codoc-os/django-opensearch-dsl/blob/master/LICENSE)
 [![codecov](https://codecov.io/gh/Codoc-os/django-opensearch-dsl/branch/master/graph/badge.svg)](https://codecov.io/gh/Codoc-os/django-opensearch-dsl)
 [![CodeFactor](https://www.codefactor.io/repository/github/Codoc-os/django-opensearch-dsl/badge)](https://www.codefactor.io/repository/github/Codoc-os/django-opensearch-dsl)
 
 **Django Opensearch DSL** is a package that allows the indexing of Django models in opensearch. It is built as a thin
-wrapper around [`opensearch-dsl-py`](https://github.com/opensearch-project/opensearch-dsl-py)
-so you can use all the features developed by the `opensearch-dsl` team.
+wrapper around [`opensearch-py`](https://github.com/opensearch-project/opensearch-py)
+so you can use all the features developed by the `opensearch-py` team.
 
 You can view the full documentation
 at [https://django-opensearch-dsl.readthedocs.io](https://django-opensearch-dsl.readthedocs.io/en/latest/).
 
 ## Features
 
-- Based on [`opensearch-dsl-py`](https://github.com/opensearch-project/opensearch-dsl-py) so you can make queries with
+- Based on [`opensearch-py`](https://github.com/opensearch-project/opensearch-py) so you can make queries with
   the [`Search`](https://elasticsearch-dsl.readthedocs.io/en/latest/search_dsl.html#the-search-object)
   object.
 - Management commands for creating, deleting, and populating indices and documents.
 - Opensearch auto mapping from Django models fields.
 - Complex field type support (`ObjectField`, `NestedField`).
 - Index fast using `parallel` indexing.
 
 ## Requirements
 
 `django-opensearch-dsl` only support the supported version of each dependency (mainstream & lts).
 
 * `Python>=3.7`
 * `django>=3.2`
-* `opensearch-dsl>=1.0.0, <3.0.0`
+* `opensearch-py>=1.0.0, <3.0.0`
 * `python-dateutil~=2.8.2`
 
 ## Installation and Configuration
 
 The easiest way to install `django-opensearch-dsl` is through `pip`:
 
 * `pip install django-opensearch-dsl`
@@ -58,15 +58,15 @@
         'http_auth': ("admin", "password"),
         'timeout': 120,
     },
 }
 ```
 
 `OPENSEARCH_DSL` is then passed
-to [`opensearch_dsl_py.connections.configure`](http://elasticsearch-dsl.readthedocs.io/en/stable/configuration.html#multiple-clusters)
+to [`opensearchpy.connection.connections.configure`](http://elasticsearch-dsl.readthedocs.io/en/stable/configuration.html#multiple-clusters)
 .
 
 ## Create Document Classes
 
 To index instances of the following model :
 
 ```python
```

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl/apps.py` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.apps import AppConfig
 from django.conf import settings
 from django.utils.module_loading import import_string
 
-from opensearch_dsl.connections import connections
+from opensearchpy.connection.connections import connections
 
 
 class DODConfig(AppConfig):
     """Django Opensearch DSL Appconfig."""
 
     name = "django_opensearch_dsl"
     verbose_name = "django-opensearch-dsl"
```

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl/documents.py` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl/documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from collections import deque
 from functools import partial
 from typing import Optional, Iterable
 
 from django.db import models
 from django.db.models import QuerySet, Q
-from opensearch_dsl import Document as DSLDocument
+from opensearchpy.helpers.document import Document as DSLDocument
 from opensearchpy.helpers import bulk, parallel_bulk
 
 from . import fields
 from .apps import DODConfig
 from .exceptions import ModelFieldNotMappedError
 from .management.enums import OpensearchAction
 from .search import Search
```

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl/fields.py` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Iterable
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.db.models.fields.files import FieldFile
 from django.utils.encoding import force_str
 from django.utils.functional import Promise
-from opensearch_dsl import field as fields
+from opensearchpy.helpers import field as fields
 
 from .exceptions import VariableLookupError
 
 __all__ = [
     "DODField",
     "ObjectField",
     "ListField",
```

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl/indices.py` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl/indices.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from copy import deepcopy
 
-from opensearch_dsl import Index as DSLIndex
+from opensearchpy.helpers.index import Index as DSLIndex
 
 from .apps import DODConfig
 from .registries import registry
 
 
 class Index(DSLIndex):
     """Creates an index and makes a deep copy of default index settings."""
```

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl/management/commands/opensearch.py` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl/management/commands/opensearch.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl/management/enums.py` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl/management/enums.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl/management/types.py` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl/management/types.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl/registries.py` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl/registries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import defaultdict
 from copy import deepcopy
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.exceptions import ImproperlyConfigured
-from opensearch_dsl import AttrDict
+from opensearchpy.helpers.utils import AttrDict
 
 from .apps import DODConfig
 from .exceptions import RedeclaredFieldError
 
 
 class DocumentRegistry:
     """Registry of models classes to a set of Document classes."""
@@ -84,15 +84,18 @@
         self.register(index=document._index, doc_class=document)  # noqa
 
         return document
 
     def _get_related_doc(self, instance):
         for model in self._related_models.get(instance.__class__, []):
             for doc in self._models[model]:
-                if instance.__class__ in doc.django.related_models:
+                if (
+                    instance.__class__ in doc.django.related_models
+                    or instance.__class__.__base__ in doc.django.related_models
+                ):
                     yield doc
 
     def update_related(self, instance, action="index", **kwargs):
         """Update documents related to `instance`.
 
         Related documents are found using the `get_instances_from_related()`
         method of each Document classes including the instance's Model is
@@ -141,14 +144,19 @@
             return
 
         if instance.__class__ in self._models:
             for doc in self._models[instance.__class__]:
                 if not doc.django.ignore_signals:
                     doc().update(instance, action, **kwargs)
 
+        if instance.__class__.__base__ in self._models:
+            for doc in self._models[instance.__class__.__base__]:
+                if not doc.django.ignore_signals:
+                    doc().update(instance, action, **kwargs)
+
     def delete(self, instance, **kwargs):
         """Delete all the opensearch documents attached to this model.
 
         Only delete if settings' `OPENSEARCH_DSL_AUTOSYNC` is `True` and
         `Document'`s `ignore_signals` is `False`.
         """
         self.update(instance, action="delete", **kwargs)
```

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl/search.py` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from django.db.models import Case, When
 from django.db.models.fields import IntegerField
 
-from opensearch_dsl import Search as DSLSearch
-from opensearch_dsl.connections import connections
+from opensearchpy.helpers.search import Search as DSLSearch
+from opensearchpy.connection.connections import connections
 
 
 class Search(DSLSearch):
-    """Subclass of `opensearch_dsl.Search` with some utility methods."""
+    """Subclass of `opensearchpy.helpers.search.Search` with some utility methods."""
 
     def __init__(self, **kwargs):
         self._model = kwargs.pop("model", None)
         super(Search, self).__init__(**kwargs)
 
     def _clone(self):
         s = super(Search, self)._clone()
```

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl/signals.py` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl/signals.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl.egg-info/PKG-INFO` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-opensearch-dsl
-Version: 0.5.0
-Summary: Wrapper around opensearch-dsl-py for django models
+Version: 0.5.1
+Summary: Wrapper around opensearch-py for django models
 Home-page: https://github.com/qcoumes/django-opensearch-dsl
 Author: Quentin Coumes (Codoc)
 Author-email: coumes.quentin@gmail.com
 License: Apache Software License 2.0
-Keywords: django elasticsearch elasticsearch-dsl opensearch opensearch-dsl
+Keywords: django elasticsearch elasticsearch-dsl opensearch opensearch-dsl opensearch-py
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -33,37 +33,37 @@
 [![Python 3.7+](https://img.shields.io/badge/Python-3.6+-brightgreen.svg)](#)
 [![Django 3.2+](https://img.shields.io/badge/Django-2.1+-brightgreen.svg)](#)
 [![License Apache 2](https://img.shields.io/badge/license-Apache%202-brightgreen.svg)](https://github.com/Codoc-os/django-opensearch-dsl/blob/master/LICENSE)
 [![codecov](https://codecov.io/gh/Codoc-os/django-opensearch-dsl/branch/master/graph/badge.svg)](https://codecov.io/gh/Codoc-os/django-opensearch-dsl)
 [![CodeFactor](https://www.codefactor.io/repository/github/Codoc-os/django-opensearch-dsl/badge)](https://www.codefactor.io/repository/github/Codoc-os/django-opensearch-dsl)
 
 **Django Opensearch DSL** is a package that allows the indexing of Django models in opensearch. It is built as a thin
-wrapper around [`opensearch-dsl-py`](https://github.com/opensearch-project/opensearch-dsl-py)
-so you can use all the features developed by the `opensearch-dsl` team.
+wrapper around [`opensearch-py`](https://github.com/opensearch-project/opensearch-py)
+so you can use all the features developed by the `opensearch-py` team.
 
 You can view the full documentation
 at [https://django-opensearch-dsl.readthedocs.io](https://django-opensearch-dsl.readthedocs.io/en/latest/).
 
 ## Features
 
-- Based on [`opensearch-dsl-py`](https://github.com/opensearch-project/opensearch-dsl-py) so you can make queries with
+- Based on [`opensearch-py`](https://github.com/opensearch-project/opensearch-py) so you can make queries with
   the [`Search`](https://elasticsearch-dsl.readthedocs.io/en/latest/search_dsl.html#the-search-object)
   object.
 - Management commands for creating, deleting, and populating indices and documents.
 - Opensearch auto mapping from Django models fields.
 - Complex field type support (`ObjectField`, `NestedField`).
 - Index fast using `parallel` indexing.
 
 ## Requirements
 
 `django-opensearch-dsl` only support the supported version of each dependency (mainstream & lts).
 
 * `Python>=3.7`
 * `django>=3.2`
-* `opensearch-dsl>=1.0.0, <3.0.0`
+* `opensearch-py>=1.0.0, <3.0.0`
 * `python-dateutil~=2.8.2`
 
 ## Installation and Configuration
 
 The easiest way to install `django-opensearch-dsl` is through `pip`:
 
 * `pip install django-opensearch-dsl`
@@ -84,15 +84,15 @@
         'http_auth': ("admin", "password"),
         'timeout': 120,
     },
 }
 ```
 
 `OPENSEARCH_DSL` is then passed
-to [`opensearch_dsl_py.connections.configure`](http://elasticsearch-dsl.readthedocs.io/en/stable/configuration.html#multiple-clusters)
+to [`opensearchpy.connection.connections.configure`](http://elasticsearch-dsl.readthedocs.io/en/stable/configuration.html#multiple-clusters)
 .
 
 ## Create Document Classes
 
 To index instances of the following model :
 
 ```python
@@ -147,14 +147,22 @@
         # Paginate the django queryset used to populate the index with the specified size
         # This per-Document setting overrides settings.OPENSEARCH_DSL_QUERYSET_PAGINATION.
         queryset_pagination = 5000
 ```
 
 # Changelog
 
+### 0.5.1 (2023-05-18)
+
+* Change references from `opensearch-dsl-py` to `opensearch-py`.  
+  This follow the deprecation notice on the
+  [`opensearch-dsl-py`](https://github.com/opensearch-project/opensearch-dsl-py) project. Its features are now directly
+  included in `opensearch-py`.  
+  ([#33](https://github.com/Codoc-os/django-opensearch-dsl/issues/33), Contributed by [Jacob Kausler](https://github.com/jakekausler)).
+
 ## 0.5.0 (2022-11-19)
 
 * `get_indexing_queryset()` now order unordered QuerySet by their PK.
   ([#29](https://github.com/Codoc-os/django-opensearch-dsl/issues/29), Contributed by [Cédric Raud](https://github.com/cedricraud)).
 * `keep_order` argument of `django_opensearch_dsl.search.Search.to_queryset` now default to `True`
   to be in line with the documentation ([#27](https://github.com/Codoc-os/django-opensearch-dsl/issues/27)).
```

### Comparing `django-opensearch-dsl-0.5.0/django_opensearch_dsl.egg-info/SOURCES.txt` & `django-opensearch-dsl-0.5.1/django_opensearch_dsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.5.0/docs/CHANGELOG.md` & `django-opensearch-dsl-0.5.1/docs/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+### 0.5.1 (2023-05-18)
+
+* Change references from `opensearch-dsl-py` to `opensearch-py`.  
+  This follow the deprecation notice on the
+  [`opensearch-dsl-py`](https://github.com/opensearch-project/opensearch-dsl-py) project. Its features are now directly
+  included in `opensearch-py`.  
+  ([#33](https://github.com/Codoc-os/django-opensearch-dsl/issues/33), Contributed by [Jacob Kausler](https://github.com/jakekausler)).
+
 ## 0.5.0 (2022-11-19)
 
 * `get_indexing_queryset()` now order unordered QuerySet by their PK.
   ([#29](https://github.com/Codoc-os/django-opensearch-dsl/issues/29), Contributed by [Cédric Raud](https://github.com/cedricraud)).
 * `keep_order` argument of `django_opensearch_dsl.search.Search.to_queryset` now default to `True`
   to be in line with the documentation ([#27](https://github.com/Codoc-os/django-opensearch-dsl/issues/27)).
```

### Comparing `django-opensearch-dsl-0.5.0/setup.cfg` & `django-opensearch-dsl-0.5.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 	opensearch10: DJANGO_OS_PORT=9210
 	opensearch20: DJANGO_OS_PORT=9220
 deps = 
 	-rrequirements.txt
 	django32: django>=3.2.0,<3.3.0
 	django40: django>=4.0.0,<4.1.0
 	django41: django>=4.1.0,<4.2.0
-	opensearch10: opensearch-dsl>=1.0.0, <2.0.0
-	opensearch20: opensearch-dsl>=2.0.0, <3.0.0
+	opensearch10: opensearch-py>=2.2.0
+	opensearch20: opensearch-py>=2.2.0
 	pycodestyle
 	pydocstyle
 	pytest-cov
 commands = 
 	pycodestyle django_opensearch_dsl
 	-pydocstyle --count django_opensearch_dsl
 	python3 manage.py migrate
```

### Comparing `django-opensearch-dsl-0.5.0/setup.py` & `django-opensearch-dsl-0.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 ]
 LONG_DESCRIPTION = (
     codecs.open(os.path.join(DIRNAME, 'README.md'), encoding='utf-8').read()
     + '\n'
     + codecs.open(os.path.join(DIRNAME, 'docs/CHANGELOG.md'), encoding='utf-8').read()
 )
 REQUIREMENTS = [
-    'opensearch-dsl>=1.0.0, <3.0.0',
+    'opensearch-py>=2.2.0',
     'dateutils'
 ]
 
 setup(
     name='django-opensearch-dsl',
-    version='0.5.0',
-    description="""Wrapper around opensearch-dsl-py for django models""",
+    version='0.5.1',
+    description="""Wrapper around opensearch-py for django models""",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author='Quentin Coumes (Codoc)',
     author_email='coumes.quentin@gmail.com',
     url='https://github.com/qcoumes/django-opensearch-dsl',
     packages=['django_opensearch_dsl'],
     include_package_data=True,
     install_requires=REQUIREMENTS,
     license="Apache Software License 2.0",
-    keywords='django elasticsearch elasticsearch-dsl opensearch opensearch-dsl',
+    keywords='django elasticsearch elasticsearch-dsl opensearch opensearch-dsl opensearch-py',
     classifiers=CLASSIFIERS,
 )
```

