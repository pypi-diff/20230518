# Comparing `tmp/vecs-0.2.1.tar.gz` & `tmp/vecs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecs-0.2.1.tar", last modified: Wed May 17 19:20:50 2023, max compression
+gzip compressed data, was "vecs-0.2.2.tar", last modified: Wed May 17 23:24:14 2023, max compression
```

## Comparing `vecs-0.2.1.tar` & `vecs-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 19:20:50.105667 vecs-0.2.1/
--rw-r--r--   0 oliverrice   (501) staff       (20)      742 2023-05-17 19:20:50.105527 vecs-0.2.1/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)     6055 2023-05-17 18:27:20.000000 vecs-0.2.1/README.md
--rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-05-12 13:47:40.000000 vecs-0.2.1/pyproject.toml
--rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-05-17 19:20:50.105715 vecs-0.2.1/setup.cfg
--rw-r--r--   0 oliverrice   (501) staff       (20)     2188 2023-05-17 19:19:05.000000 vecs-0.2.1/setup.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 19:20:50.103492 vecs-0.2.1/src/
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 19:20:50.104435 vecs-0.2.1/src/vecs/
--rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-05-17 19:10:32.000000 vecs-0.2.1/src/vecs/__init__.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     1686 2023-05-16 19:39:23.000000 vecs-0.2.1/src/vecs/client.py
--rw-r--r--   0 oliverrice   (501) staff       (20)    13522 2023-05-17 19:04:04.000000 vecs-0.2.1/src/vecs/collection.py
--rw-r--r--   0 oliverrice   (501) staff       (20)      491 2023-05-16 18:21:37.000000 vecs-0.2.1/src/vecs/exc.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 19:20:50.105341 vecs-0.2.1/src/vecs.egg-info/
--rw-r--r--   0 oliverrice   (501) staff       (20)      742 2023-05-17 19:20:50.000000 vecs-0.2.1/src/vecs.egg-info/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)      271 2023-05-17 19:20:50.000000 vecs-0.2.1/src/vecs.egg-info/SOURCES.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-05-17 19:20:50.000000 vecs-0.2.1/src/vecs.egg-info/dependency_links.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)      146 2023-05-17 19:20:50.000000 vecs-0.2.1/src/vecs.egg-info/requires.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-05-17 19:20:50.000000 vecs-0.2.1/src/vecs.egg-info/top_level.txt
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 23:24:14.207342 vecs-0.2.2/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      742 2023-05-17 23:24:14.207219 vecs-0.2.2/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)     6013 2023-05-17 19:24:32.000000 vecs-0.2.2/README.md
+-rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-05-12 13:47:40.000000 vecs-0.2.2/pyproject.toml
+-rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-05-17 23:24:14.207394 vecs-0.2.2/setup.cfg
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2221 2023-05-17 23:23:18.000000 vecs-0.2.2/setup.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 23:24:14.204907 vecs-0.2.2/src/
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 23:24:14.206354 vecs-0.2.2/src/vecs/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-05-17 23:23:39.000000 vecs-0.2.2/src/vecs/__init__.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     1686 2023-05-16 19:39:23.000000 vecs-0.2.2/src/vecs/client.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)    13522 2023-05-17 19:04:04.000000 vecs-0.2.2/src/vecs/collection.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)      491 2023-05-16 18:21:37.000000 vecs-0.2.2/src/vecs/exc.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 23:24:14.207053 vecs-0.2.2/src/vecs.egg-info/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      742 2023-05-17 23:24:14.000000 vecs-0.2.2/src/vecs.egg-info/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)      271 2023-05-17 23:24:14.000000 vecs-0.2.2/src/vecs.egg-info/SOURCES.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-05-17 23:24:14.000000 vecs-0.2.2/src/vecs.egg-info/dependency_links.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)      157 2023-05-17 23:24:14.000000 vecs-0.2.2/src/vecs.egg-info/requires.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-05-17 23:24:14.000000 vecs-0.2.2/src/vecs.egg-info/top_level.txt
```

### Comparing `vecs-0.2.1/PKG-INFO` & `vecs-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.2.1
+Version: 0.2.2
 Summary: pgvector client
 Home-page: https://github.com/olirice/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `vecs-0.2.1/README.md` & `vecs-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # vecs
 
 <p>
 
 <p>
     <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="Python version" height="18"></a>
-  <a href="https://badge.fury.io/py/vecs"><img src="https://badge.fury.io/py/vecs.svg" alt="PyPI version" height="18"></a>
+    <a href="https://badge.fury.io/py/vecs"><img src="https://badge.fury.io/py/vecs.svg" alt="PyPI version" height="18"></a>
     <a href="https://github.com/olirice/vecs/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/markdown-subtemplate.svg" alt="License" height="18"></a>
     <a href="https://pypi.org/project/vecs/"><img src="https://img.shields.io/pypi/dm/vecs.svg" alt="Download count" height="18"></a>
 </p>
 
 ---
 
 **Documentation**: <a href="https://olirice.github.io/vecs/api/" target="_blank">https://olirice.github.io/vecs/api/</a>
@@ -146,18 +146,17 @@
 
 If you aren't sure which to use, stick with the default (cosine_distance) by omitting the parameter i.e.
 
 ```
 docs.create_index()
 ```
 
-!!! note
-    The time required to create an index grows with the number of records and size of vectors.
-    For a few thousand records expect sub-minute a response in under a minute. It may take a few
-    minutes for larger collections.
+Note that The time required to create an index grows with the number of records and size of vectors.
+For a few thousand records expect sub-minute a response in under a minute. It may take a few
+minutes for larger collections.
 
 ## Query
 
 Given a collection `docs` with several records:
 
 ### Basic
 
@@ -172,22 +171,21 @@
     include_value=False,         # should distance measure values be returned?
     include_metadata=False,      # should record metadata be returned?
 )
 ```
 
 Which returns a list of vector record `ids`.
 
-!!! note
-    Indexes are essential for good performance. See [creating an index](#create-an-index) for more info.
+Indexes are essential for good performance. See [creating an index](#create-an-index) for more info.
 
-    If you do not create an index, every query will return a warning
-    ```
-    query does not have a covering index for cosine_similarity. See Collection.create_index
-    ```
-    that incldues the `IndexMeasure` you should index.
+If you do not create an index, every query will return a warning
+```
+query does not have a covering index for cosine_similarity. See Collection.create_index
+```
+that incldues the `IndexMeasure` you should index.
 
 
 ### Metadata Filtering
 
 The metadata that is associated with each record can also be filtered during a query.
 
 As an example, `{"year": {"$eq": 2005}}` filters a `year` metadata key to be equal to 2005
```

#### html2text {}

```diff
@@ -41,24 +41,24 @@
 index the collection to be queried by cosine distance docs.create_index
 (measure=vecs.IndexMeasure.cosine_distance) ``` Available options for query
 `measure` are: - `vecs.IndexMeasure.cosine_distance` -
 `vecs.IndexMeasure.l2_distance` - `vecs.IndexMeasure.max_inner_product` which
 correspond to different methods for comparing query vectors to the vectors in
 the database. If you aren't sure which to use, stick with the default
 (cosine_distance) by omitting the parameter i.e. ``` docs.create_index() ```
-!!! note The time required to create an index grows with the number of records
+Note that The time required to create an index grows with the number of records
 and size of vectors. For a few thousand records expect sub-minute a response in
 under a minute. It may take a few minutes for larger collections. ## Query
 Given a collection `docs` with several records: ### Basic The simplest form of
 search is to provide a query vector. ```python docs.query( query_vector=
 [0.4,0.5,0.6], # required limit=5, # number of records to return filters={}, #
 metadata filters measure="cosine_distance", # distance measure to use
 include_value=False, # should distance measure values be returned?
 include_metadata=False, # should record metadata be returned? ) ``` Which
-returns a list of vector record `ids`. !!! note Indexes are essential for good
+returns a list of vector record `ids`. Indexes are essential for good
 performance. See [creating an index](#create-an-index) for more info. If you do
 not create an index, every query will return a warning ``` query does not have
 a covering index for cosine_similarity. See Collection.create_index ``` that
 incldues the `IndexMeasure` you should index. ### Metadata Filtering The
 metadata that is associated with each record can also be filtered during a
 query. As an example, `{"year": {"$eq": 2005}}` filters a `year` metadata key
 to be equal to 2005 In context: ```python docs.query( query_vector=
```

### Comparing `vecs-0.2.1/setup.py` & `vecs-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,20 @@
     logging.warning("'%s' not found in '%s'", key, module_path)
     raise KeyError(key)
 
 
 check_python_version()
 
 
-REQUIRES = ["pgvector==0.1.*", "sqlalchemy==2.*", "psycopg2-binary==2.9.*"]
+REQUIRES = [
+    "pgvector==0.1.*",
+    "sqlalchemy==2.*",
+    "psycopg2-binary==2.9.*",
+    "flupy==1.*",
+]
 
 
 setuptools.setup(
     name=read_package_variable("__project__"),
     version=read_package_variable("__version__"),
     description="pgvector client",
     url="https://github.com/olirice/vecs",
```

### Comparing `vecs-0.2.1/src/vecs/client.py` & `vecs-0.2.2/src/vecs/client.py`

 * *Files identical despite different names*

### Comparing `vecs-0.2.1/src/vecs/collection.py` & `vecs-0.2.2/src/vecs/collection.py`

 * *Files identical despite different names*

### Comparing `vecs-0.2.1/src/vecs.egg-info/PKG-INFO` & `vecs-0.2.2/src/vecs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.2.1
+Version: 0.2.2
 Summary: pgvector client
 Home-page: https://github.com/olirice/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

