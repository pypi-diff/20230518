# Comparing `tmp/monarch_py-0.8.0.tar.gz` & `tmp/monarch_py-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.8.0.tar", max compression
+gzip compressed data, was "monarch_py-0.8.1.tar", max compression
```

## Comparing `monarch_py-0.8.0.tar` & `monarch_py-0.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      955 2023-05-17 20:08:53.342423 monarch_py-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       77 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     1630 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/association_type_mappings.yaml
--rw-r--r--   0        0        0     7377 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0    11736 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     9463 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3300 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    20371 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8909 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2343 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     4697 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     9031 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3330 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     4052 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/utils/association_type_utils.py
--rw-r--r--   0        0        0     3985 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4937 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      955 2023-05-17 23:43:22.516925 monarch_py-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1630 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     7377 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0    11736 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     9463 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3300 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    20371 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-05-17 23:43:22.516925 monarch_py-0.8.1/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-05-17 23:43:22.520925 monarch_py-0.8.1/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     4697 2023-05-17 23:43:22.520925 monarch_py-0.8.1/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:43:22.520925 monarch_py-0.8.1/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-17 23:43:22.520925 monarch_py-0.8.1/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     9031 2023-05-17 23:43:22.520925 monarch_py-0.8.1/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3330 2023-05-17 23:43:22.520925 monarch_py-0.8.1/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:43:22.520925 monarch_py-0.8.1/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     4145 2023-05-17 23:43:22.520925 monarch_py-0.8.1/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3985 2023-05-17 23:43:22.520925 monarch_py-0.8.1/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4937 2023-05-17 23:43:22.520925 monarch_py-0.8.1/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.8.1/PKG-INFO
```

### Comparing `monarch_py-0.8.0/pyproject.toml` & `monarch_py-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.8.0"
+version = "0.8.1"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.8.0/src/monarch_py/association_type_mappings.yaml` & `monarch_py-0.8.1/src/monarch_py/association_type_mappings.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/cli.py` & `monarch_py-0.8.1/src/monarch_py/cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/datamodels/model.py` & `monarch_py-0.8.1/src/monarch_py/datamodels/model.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.8.1/src/monarch_py/datamodels/model.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/datamodels/solr.py` & `monarch_py-0.8.1/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.8.1/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.8.1/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.8.1/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.8.1/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.8.1/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.8.1/src/monarch_py/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/service/solr_service.py` & `monarch_py-0.8.1/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/solr_cli.py` & `monarch_py-0.8.1/src/monarch_py/solr_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/sql_cli.py` & `monarch_py-0.8.1/src/monarch_py/sql_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/utils/association_type_utils.py` & `monarch_py-0.8.1/src/monarch_py/utils/association_type_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     @staticmethod
     def get_mappings():
         if AssociationTypeMappings.__instance is None:
             AssociationTypeMappings()
         return AssociationTypeMappings.__instance.mappings
 
     def get_mapping(self, association_type: AssociationTypeEnum):
+        if AssociationTypeMappings.__instance is None:
+            AssociationTypeMappings()
         for mapping in self.mappings:
             if mapping.association_type == association_type:
                 return mapping
 
     def load_mappings(self):
         mapping_data = pkgutil.get_data(
             __package__, "../association_type_mappings.yaml"
```

### Comparing `monarch_py-0.8.0/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.8.1/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/src/monarch_py/utils/utils.py` & `monarch_py-0.8.1/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.0/PKG-INFO` & `monarch_py-0.8.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.8.0
+Version: 0.8.1
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

