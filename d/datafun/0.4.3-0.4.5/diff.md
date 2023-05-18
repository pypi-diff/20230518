# Comparing `tmp/datafun-0.4.3.tar.gz` & `tmp/datafun-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafun-0.4.3.tar", last modified: Tue Sep 27 14:26:32 2022, max compression
+gzip compressed data, was "datafun-0.4.5.tar", last modified: Thu May 18 14:31:13 2023, max compression
```

## Comparing `datafun-0.4.3.tar` & `datafun-0.4.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:26:32.517990 datafun-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-09-27 14:26:16.000000 datafun-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    29636 2022-09-27 14:26:32.517990 datafun-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    29073 2022-09-27 14:26:16.000000 datafun-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:26:32.517990 datafun-0.4.3/datafun/
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-09-27 14:26:16.000000 datafun-0.4.3/datafun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-09-27 14:26:16.000000 datafun-0.4.3/datafun/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    32178 2022-09-27 14:26:16.000000 datafun-0.4.3/datafun/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:26:32.517990 datafun-0.4.3/datafun/sources/
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-09-27 14:26:16.000000 datafun-0.4.3/datafun/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4687 2022-09-27 14:26:16.000000 datafun-0.4.3/datafun/sources/elk.py
--rw-r--r--   0 runner    (1001) docker     (121)     7705 2022-09-27 14:26:16.000000 datafun-0.4.3/datafun/sources/gcs.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-09-27 14:26:16.000000 datafun-0.4.3/datafun/sources/iterable.py
--rw-r--r--   0 runner    (1001) docker     (121)     5392 2022-09-27 14:26:16.000000 datafun-0.4.3/datafun/sources/local_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-09-27 14:26:16.000000 datafun-0.4.3/datafun/sources/rest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-09-27 14:26:16.000000 datafun-0.4.3/datafun/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:26:32.517990 datafun-0.4.3/datafun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    29636 2022-09-27 14:26:32.000000 datafun-0.4.3/datafun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-27 14:26:32.000000 datafun-0.4.3/datafun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 14:26:32.000000 datafun-0.4.3/datafun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-09-27 14:26:32.000000 datafun-0.4.3/datafun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-27 14:26:32.000000 datafun-0.4.3/datafun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-27 14:26:16.000000 datafun-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 14:26:32.517990 datafun-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-09-27 14:26:16.000000 datafun-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:31:13.345879 datafun-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-18 14:31:04.000000 datafun-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-05-18 14:31:13.345879 datafun-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29266 2023-05-18 14:31:04.000000 datafun-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:31:13.345879 datafun-0.4.5/datafun/
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-18 14:31:04.000000 datafun-0.4.5/datafun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-18 14:31:04.000000 datafun-0.4.5/datafun/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32178 2023-05-18 14:31:04.000000 datafun-0.4.5/datafun/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:31:13.345879 datafun-0.4.5/datafun/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-18 14:31:04.000000 datafun-0.4.5/datafun/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-18 14:31:04.000000 datafun-0.4.5/datafun/sources/elk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-18 14:31:04.000000 datafun-0.4.5/datafun/sources/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-18 14:31:04.000000 datafun-0.4.5/datafun/sources/iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-18 14:31:04.000000 datafun-0.4.5/datafun/sources/local_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-18 14:31:04.000000 datafun-0.4.5/datafun/sources/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-18 14:31:04.000000 datafun-0.4.5/datafun/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:31:13.345879 datafun-0.4.5/datafun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-05-18 14:31:13.000000 datafun-0.4.5/datafun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-18 14:31:13.000000 datafun-0.4.5/datafun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:31:13.000000 datafun-0.4.5/datafun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 14:31:13.000000 datafun-0.4.5/datafun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 14:31:13.000000 datafun-0.4.5/datafun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-18 14:31:04.000000 datafun-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 14:31:13.345879 datafun-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-18 14:31:04.000000 datafun-0.4.5/setup.py
```

### Comparing `datafun-0.4.3/LICENSE` & `datafun-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datafun-0.4.3/PKG-INFO` & `datafun-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafun
-Version: 0.4.3
+Version: 0.4.5
 Summary: datafun brings the fun back to data pipelines
 Home-page: https://github.com/aitechnologies-it/datafun
 Author: Luigi Di Sotto, Diego Giorgini, Saeed Choobani
 Author-email: luigi.disotto@aitechnologies.it, diego.giorgini@aitechnologies.it, saeed.choobani@aitechnologies.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -292,14 +292,15 @@
 | **port**          | str                   | Yes      |            | Elastic host port                                                |
 | **username**      | str                   | Yes      |            | Elastic authentication username                                  |
 | **password**      | str                   | Yes      |            | Elastic authentication password                                  |
 | **index**         | str                   | Yes      |            | Elastic index to query                                           |
 | **start_isodate** | str (ISO datetime)    | Yes      |            | Elastic start date range with format: "2021-09-15T10:00:00.000Z" |
 | **end_isodate**   | str (ISO datetime)    | Yes      |            | Elastic end date range with format: "2021-09-15T10:00:00.000Z"   |
 | **date_field**    | str                   | No       | @timestamp | Elastic date field. Can be nested into list, eg. "messages.date" |
+| **date_field_separator** | str            | No       | .          | Separator for date_field used to split the path. Use different ones to NOT split and consider date_field as single field |
 
 **Returned element type**: ```dict```. Each element is a document matching the given query.
 
 ## RESTDataset
 
 | Name              | Type                            | Required | Default                         | Description                                                                                                                              |
 |-------------------|---------------------------------|----------|---------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `datafun-0.4.3/README.md` & `datafun-0.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -278,14 +278,15 @@
 | **port**          | str                   | Yes      |            | Elastic host port                                                |
 | **username**      | str                   | Yes      |            | Elastic authentication username                                  |
 | **password**      | str                   | Yes      |            | Elastic authentication password                                  |
 | **index**         | str                   | Yes      |            | Elastic index to query                                           |
 | **start_isodate** | str (ISO datetime)    | Yes      |            | Elastic start date range with format: "2021-09-15T10:00:00.000Z" |
 | **end_isodate**   | str (ISO datetime)    | Yes      |            | Elastic end date range with format: "2021-09-15T10:00:00.000Z"   |
 | **date_field**    | str                   | No       | @timestamp | Elastic date field. Can be nested into list, eg. "messages.date" |
+| **date_field_separator** | str            | No       | .          | Separator for date_field used to split the path. Use different ones to NOT split and consider date_field as single field |
 
 **Returned element type**: ```dict```. Each element is a document matching the given query.
 
 ## RESTDataset
 
 | Name              | Type                            | Required | Default                         | Description                                                                                                                              |
 |-------------------|---------------------------------|----------|---------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `datafun-0.4.3/datafun/__init__.py` & `datafun-0.4.5/datafun/__init__.py`

 * *Files identical despite different names*

### Comparing `datafun-0.4.3/datafun/cache.py` & `datafun-0.4.5/datafun/cache.py`

 * *Files identical despite different names*

### Comparing `datafun-0.4.3/datafun/dataset.py` & `datafun-0.4.5/datafun/dataset.py`

 * *Files identical despite different names*

### Comparing `datafun-0.4.3/datafun/sources/__init__.py` & `datafun-0.4.5/datafun/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `datafun-0.4.3/datafun/sources/elk.py` & `datafun-0.4.5/datafun/sources/elk.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     port: int
     username: str
     password: str
     index: str
     start_isodate: str
     end_isodate: str
     date_field: str = "@timestamp"
+    date_field_separator: str = "."
 
 
 class ELKDataset(DatasetSource):
     def __init__(self, config: ELKDatasetConfig, **kwargs):
         super().__init__(config=config, **kwargs)
 
         self.es = Elasticsearch(
@@ -87,20 +88,19 @@
 
         xs = dl.get(query, 'query.bool.filter')
         if xs is None:
             raise ValueError(f'Field query.bool.filter has not been found.')
         if not isinstance(xs, List):
             raise TypeError(f'Field query.bool.filter must be of type List, but found of type {type(xs)}')
 
+        sep = self.config.date_field_separator
         for idx, obj in enumerate(xs):
             if dl.has(obj, "range"):
-                obj["range"][self.config.date_field]["gte"] = self.config.start_isodate
-                obj["range"][self.config.date_field]["lte"] = self.config.end_isodate
-                # obj = dl.update(obj, path=date_field_gte, value=self.config.start_isodate)
-                # obj = dl.update(obj, path=date_field_lte, value=self.config.end_isodate)
+                obj = dl.update(obj, f"range{sep}{self.config.date_field}{sep}gte", value=self.config.start_isodate, sep=sep)
+                obj = dl.update(obj, f"range{sep}{self.config.date_field}{sep}lte", value=self.config.end_isodate, sep=sep)
                 if not obj:
                     raise ValueError(f'{self.config.date_field}.lte or {self.config.date_field}.lte fields can\'t be updated, e.g. check '
                                     'if they exist in the query.')
                 xs[idx] = obj
 
         query = dl.update(query, path='query.bool.filter', value=xs)
         return query
```

### Comparing `datafun-0.4.3/datafun/sources/gcs.py` & `datafun-0.4.5/datafun/sources/gcs.py`

 * *Files identical despite different names*

### Comparing `datafun-0.4.3/datafun/sources/iterable.py` & `datafun-0.4.5/datafun/sources/iterable.py`

 * *Files identical despite different names*

### Comparing `datafun-0.4.3/datafun/sources/local_file.py` & `datafun-0.4.5/datafun/sources/local_file.py`

 * *Files identical despite different names*

### Comparing `datafun-0.4.3/datafun/sources/rest.py` & `datafun-0.4.5/datafun/sources/rest.py`

 * *Files identical despite different names*

### Comparing `datafun-0.4.3/datafun/utils.py` & `datafun-0.4.5/datafun/utils.py`

 * *Files identical despite different names*

### Comparing `datafun-0.4.3/datafun.egg-info/PKG-INFO` & `datafun-0.4.5/datafun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafun
-Version: 0.4.3
+Version: 0.4.5
 Summary: datafun brings the fun back to data pipelines
 Home-page: https://github.com/aitechnologies-it/datafun
 Author: Luigi Di Sotto, Diego Giorgini, Saeed Choobani
 Author-email: luigi.disotto@aitechnologies.it, diego.giorgini@aitechnologies.it, saeed.choobani@aitechnologies.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -292,14 +292,15 @@
 | **port**          | str                   | Yes      |            | Elastic host port                                                |
 | **username**      | str                   | Yes      |            | Elastic authentication username                                  |
 | **password**      | str                   | Yes      |            | Elastic authentication password                                  |
 | **index**         | str                   | Yes      |            | Elastic index to query                                           |
 | **start_isodate** | str (ISO datetime)    | Yes      |            | Elastic start date range with format: "2021-09-15T10:00:00.000Z" |
 | **end_isodate**   | str (ISO datetime)    | Yes      |            | Elastic end date range with format: "2021-09-15T10:00:00.000Z"   |
 | **date_field**    | str                   | No       | @timestamp | Elastic date field. Can be nested into list, eg. "messages.date" |
+| **date_field_separator** | str            | No       | .          | Separator for date_field used to split the path. Use different ones to NOT split and consider date_field as single field |
 
 **Returned element type**: ```dict```. Each element is a document matching the given query.
 
 ## RESTDataset
 
 | Name              | Type                            | Required | Default                         | Description                                                                                                                              |
 |-------------------|---------------------------------|----------|---------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `datafun-0.4.3/setup.py` & `datafun-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="datafun",
-    version="0.4.3",
+    version="0.4.5",
     author="Luigi Di Sotto, Diego Giorgini, Saeed Choobani",
     author_email="luigi.disotto@aitechnologies.it, diego.giorgini@aitechnologies.it, saeed.choobani@aitechnologies.it",
     description="datafun brings the fun back to data pipelines",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aitechnologies-it/datafun",
     # packages=setuptools.find_packages(where="."),
```

