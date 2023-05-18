# Comparing `tmp/hagis-0.7.4.tar.gz` & `tmp/hagis-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.7.4.tar", last modified: Wed May 17 20:52:12 2023, max compression
+gzip compressed data, was "hagis-0.8.0.tar", last modified: Thu May 18 12:38:26 2023, max compression
```

## Comparing `hagis-0.7.4.tar` & `hagis-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 20:52:12.241524 hagis-0.7.4/
--rw-rw-rw-   0        0        0      923 2023-05-17 20:52:12.240349 hagis-0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-17 20:49:35.000000 hagis-0.7.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 20:52:12.238382 hagis-0.7.4/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-17 20:52:12.000000 hagis-0.7.4/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-17 20:52:12.000000 hagis-0.7.4/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 20:52:12.000000 hagis-0.7.4/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-17 20:52:12.000000 hagis-0.7.4/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    26722 2023-05-17 18:59:21.000000 hagis-0.7.4/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-17 16:36:21.000000 hagis-0.7.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-17 20:52:12.242391 hagis-0.7.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 12:38:26.432486 hagis-0.8.0/
+-rw-rw-rw-   0        0        0      932 2023-05-18 12:38:26.432009 hagis-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-18 12:36:24.000000 hagis-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 12:38:26.419990 hagis-0.8.0/hagis.egg-info/
+-rw-rw-rw-   0        0        0      932 2023-05-18 12:38:26.000000 hagis-0.8.0/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-18 12:38:26.000000 hagis-0.8.0/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 12:38:26.000000 hagis-0.8.0/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 12:38:26.000000 hagis-0.8.0/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    26890 2023-05-18 12:27:52.000000 hagis-0.8.0/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-18 12:36:41.000000 hagis-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 12:38:26.432486 hagis-0.8.0/setup.cfg
```

### Comparing `hagis-0.7.4/PKG-INFO` & `hagis-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.7.4
+Version: 0.8.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,16 +18,16 @@
 ```python
 from hagis import Layer, Point
 
 class City:
     objectid: int
     areaname: str
     pop2000: int
-    shape: Point
+    geometry: Point
 
 layer = Layer("https://sampleserver6.arcgisonline.com/arcgis/rest/services/USA/MapServer/0", City)
 
 for city in layer.query():
-    print(city.areaname, city.pop2000, city.shape.x, city.shape.y)
+    print(city.areaname, city.pop2000, city.geometry.x, city.geometry.y)
 ```
 
 [More examples](https://github.com/jshirota/Hagis/blob/main/demo.ipynb)
```

### Comparing `hagis-0.7.4/hagis.egg-info/PKG-INFO` & `hagis-0.8.0/hagis.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.7.4
+Version: 0.8.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,16 +18,16 @@
 ```python
 from hagis import Layer, Point
 
 class City:
     objectid: int
     areaname: str
     pop2000: int
-    shape: Point
+    geometry: Point
 
 layer = Layer("https://sampleserver6.arcgisonline.com/arcgis/rest/services/USA/MapServer/0", City)
 
 for city in layer.query():
-    print(city.areaname, city.pop2000, city.shape.x, city.shape.y)
+    print(city.areaname, city.pop2000, city.geometry.x, city.geometry.y)
 ```
 
 [More examples](https://github.com/jshirota/Hagis/blob/main/demo.ipynb)
```

### Comparing `hagis-0.7.4/hagis.py` & `hagis-0.8.0/hagis.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 class Layer(Generic[T], Iterator[T]):  # pylint: disable=too-many-instance-attributes
     """ Layer class.
 
     Args:
         Generic (T): Type argument.
     """
     def __init__(self, layer_url: str, model: Type[T] = SimpleNamespace,
-                 oid_field: str = "objectid", shape_property_name: str = "shape", **mapping: str) -> None:
+                 oid_field: str = "objectid", shape_property_name: str = "geometry", **mapping: str) -> None:
         """ Creates a new instance of the Layer class.
 
         Args:
             layer_url (str): Layer url (e.g. .../FeatureServer/0).
             model (Type[T], optional): Model to map to.  Defaults to SimpleNamespace.
             oid_field (str, optional): Name of the Object ID field.  Defaults to "objectid".
-            shape_property_name (str, optional): Name of the shape property.  Defaults to "shape".
+            shape_property_name (str, optional): Name of the geometry property.  Defaults to "geometry".
         """
         self._layer_url = layer_url
         self._model = model
         self._iterator = None
         self._oid_field = oid_field
         self._shape_property_name = shape_property_name
         self._shape_property_type = None
@@ -172,15 +172,18 @@
             if self._is_dynamic:
                 yield row  # type: ignore
             else:
                 if self._has_parameterless_constructor:
                     item = self._model()
                     row_dict = {key.lower(): value for key, value in row.__dict__.items()}
                     for property_name, field_name in self._property_name_to_lower_field.items():
-                        setattr(item, property_name, row_dict[field_name.lower()])
+                        if field_name.lower() in row_dict:
+                            setattr(item, property_name, row_dict[field_name.lower()])
+                        else:
+                            setattr(item, property_name, None)
                 else:
                     # Support for data classes and named tuples.
                     item = self._model(*row.__dict__.values())
 
                 yield item
 
     def count(self, where_clause: Union[str, Callable[[T], bool], None] = None) -> int:
```

### Comparing `hagis-0.7.4/pyproject.toml` & `hagis-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.7.4"
+version = "0.8.0"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

