# Comparing `tmp/hagis-0.8.1.tar.gz` & `tmp/hagis-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.8.1.tar", last modified: Thu May 18 16:41:33 2023, max compression
+gzip compressed data, was "hagis-0.8.2.tar", last modified: Thu May 18 20:38:51 2023, max compression
```

## Comparing `hagis-0.8.1.tar` & `hagis-0.8.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 16:41:33.092647 hagis-0.8.1/
--rw-rw-rw-   0        0        0      932 2023-05-18 16:41:33.090646 hagis-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-05-18 12:36:24.000000 hagis-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 16:41:33.089127 hagis-0.8.1/hagis.egg-info/
--rw-rw-rw-   0        0        0      932 2023-05-18 16:41:33.000000 hagis-0.8.1/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-18 16:41:33.000000 hagis-0.8.1/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 16:41:33.000000 hagis-0.8.1/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 16:41:33.000000 hagis-0.8.1/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    27388 2023-05-18 16:38:11.000000 hagis-0.8.1/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-18 16:23:12.000000 hagis-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 16:41:33.093526 hagis-0.8.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 20:38:51.938210 hagis-0.8.2/
+-rw-rw-rw-   0        0        0      932 2023-05-18 20:38:51.935635 hagis-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-18 12:36:24.000000 hagis-0.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 20:38:51.933420 hagis-0.8.2/hagis.egg-info/
+-rw-rw-rw-   0        0        0      932 2023-05-18 20:38:51.000000 hagis-0.8.2/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-18 20:38:51.000000 hagis-0.8.2/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 20:38:51.000000 hagis-0.8.2/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 20:38:51.000000 hagis-0.8.2/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    27480 2023-05-18 20:37:31.000000 hagis-0.8.2/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-18 20:37:23.000000 hagis-0.8.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 20:38:51.939205 hagis-0.8.2/setup.cfg
```

### Comparing `hagis-0.8.1/PKG-INFO` & `hagis-0.8.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.8.1
+Version: 0.8.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.8.1/hagis.egg-info/PKG-INFO` & `hagis-0.8.2/hagis.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.8.1
+Version: 0.8.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.8.1/hagis.py` & `hagis-0.8.2/hagis.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,25 +168,29 @@
         if wkid:
             kwargs["outSR"] = wkid
 
         for row in islice(self._query(where_clause, fields, record_count, max_workers, **kwargs), record_count):
             if self._is_dynamic:
                 yield row  # type: ignore
             else:
+                row_dict = {key.lower(): value for key, value in row.__dict__.items()}
+                property_dict: Dict[str, Any] = {}
+
+                for property_name, field_name in self._property_name_to_lower_field.items():
+                    if field_name in row_dict:
+                        property_dict[property_name] = row_dict[field_name]
+                    else:
+                        property_dict[property_name] = None
+
                 if self._has_parameterless_constructor:
                     item = self._model()
-                    row_dict = {key.lower(): value for key, value in row.__dict__.items()}
-                    for property_name, field_name in self._property_name_to_lower_field.items():
-                        if field_name in row_dict:
-                            setattr(item, property_name, row_dict[field_name])
-                        else:
-                            setattr(item, property_name, None)
+                    item.__dict__.update(property_dict)
                 else:
                     # Support for data classes and named tuples.
-                    item = self._model(*row.__dict__.values())
+                    item = self._model(*property_dict.values())
 
                 yield item
 
     def count(self, where_clause: Union[str, Callable[[T], bool], None] = None) -> int:
         """ Checks the number of items that match the where clause.
 
         Args:
```

### Comparing `hagis-0.8.1/pyproject.toml` & `hagis-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

