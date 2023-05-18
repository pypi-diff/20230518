# Comparing `tmp/flask_leaflet-0.1.1.tar.gz` & `tmp/flask_leaflet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_leaflet-0.1.1.tar", last modified: Thu May 18 06:41:10 2023, max compression
+gzip compressed data, was "flask_leaflet-0.1.2.tar", last modified: Thu May 18 06:46:54 2023, max compression
```

## Comparing `flask_leaflet-0.1.1.tar` & `flask_leaflet-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     4478 2023-05-18 06:24:55.459001 flask_leaflet-0.1.1/README.md
--rwxr-xr-x   0        0        0     2677 2023-05-18 06:39:38.258949 flask_leaflet-0.1.1/flask_leaflet/__init__.py
--rwxr-xr-x   0        0        0     1593 2023-05-14 08:31:30.463333 flask_leaflet-0.1.1/flask_leaflet/basic_types.py
--rwxr-xr-x   0        0        0        0 2023-05-11 15:07:50.000000 flask_leaflet-0.1.1/flask_leaflet/layers/__init__.py
--rwxr-xr-x   0        0        0     1018 2023-05-18 04:18:13.595361 flask_leaflet-0.1.1/flask_leaflet/layers/base.py
--rwxr-xr-x   0        0        0     5030 2023-05-18 04:33:07.698015 flask_leaflet-0.1.1/flask_leaflet/layers/paths.py
--rwxr-xr-x   0        0        0     9359 2023-05-15 05:42:11.854584 flask_leaflet-0.1.1/flask_leaflet/layers/raster.py
--rwxr-xr-x   0        0        0     8981 2023-05-15 06:37:46.212225 flask_leaflet-0.1.1/flask_leaflet/layers/ui.py
--rwxr-xr-x   0        0        0     2551 2023-05-18 06:27:35.626652 flask_leaflet-0.1.1/flask_leaflet/map.py
--rwxr-xr-x   0        0        0     2169 2023-05-15 06:17:34.702685 flask_leaflet-0.1.1/flask_leaflet/mixins.py
--rwxr-xr-x   0        0        0     1466 2023-05-14 03:46:14.846425 flask_leaflet-0.1.1/flask_leaflet/static/images/marker-icon.png
--rwxr-xr-x   0        0        0      618 2023-05-14 03:46:19.848035 flask_leaflet-0.1.1/flask_leaflet/static/images/marker-shadow.png
--rwxr-xr-x   0        0        0     1321 2023-05-14 07:53:24.704663 flask_leaflet-0.1.1/flask_leaflet/templates/dict_as_json.jinja
--rwxr-xr-x   0        0        0      518 2023-05-15 06:24:24.745973 flask_leaflet-0.1.1/flask_leaflet/templates/factory.html
--rwxr-xr-x   0        0        0      981 2023-05-18 06:39:27.827607 flask_leaflet-0.1.1/flask_leaflet/templates/load.html
--rwxr-xr-x   0        0        0      521 2023-05-15 06:24:44.124066 flask_leaflet-0.1.1/flask_leaflet/templates/map.html
--rwxr-xr-x   0        0        0      366 2023-05-18 06:41:10.088427 flask_leaflet-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4705 1970-01-01 00:00:00.000000 flask_leaflet-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     4478 2023-05-18 06:24:55.459001 flask_leaflet-0.1.2/README.md
+-rwxr-xr-x   0        0        0     2677 2023-05-18 06:39:38.258949 flask_leaflet-0.1.2/flask_leaflet/__init__.py
+-rwxr-xr-x   0        0        0     1593 2023-05-14 08:31:30.463333 flask_leaflet-0.1.2/flask_leaflet/basic_types.py
+-rwxr-xr-x   0        0        0        0 2023-05-11 15:07:50.000000 flask_leaflet-0.1.2/flask_leaflet/layers/__init__.py
+-rwxr-xr-x   0        0        0     1018 2023-05-18 04:18:13.595361 flask_leaflet-0.1.2/flask_leaflet/layers/base.py
+-rwxr-xr-x   0        0        0     5030 2023-05-18 04:33:07.698015 flask_leaflet-0.1.2/flask_leaflet/layers/paths.py
+-rwxr-xr-x   0        0        0     9359 2023-05-15 05:42:11.854584 flask_leaflet-0.1.2/flask_leaflet/layers/raster.py
+-rwxr-xr-x   0        0        0     8981 2023-05-15 06:37:46.212225 flask_leaflet-0.1.2/flask_leaflet/layers/ui.py
+-rwxr-xr-x   0        0        0     2551 2023-05-18 06:27:35.626652 flask_leaflet-0.1.2/flask_leaflet/map.py
+-rwxr-xr-x   0        0        0     2169 2023-05-15 06:17:34.702685 flask_leaflet-0.1.2/flask_leaflet/mixins.py
+-rwxr-xr-x   0        0        0     1466 2023-05-14 03:46:14.846425 flask_leaflet-0.1.2/flask_leaflet/static/images/marker-icon.png
+-rwxr-xr-x   0        0        0      618 2023-05-14 03:46:19.848035 flask_leaflet-0.1.2/flask_leaflet/static/images/marker-shadow.png
+-rwxr-xr-x   0        0        0     1321 2023-05-14 07:53:24.704663 flask_leaflet-0.1.2/flask_leaflet/templates/dict_as_json.jinja
+-rwxr-xr-x   0        0        0      518 2023-05-15 06:24:24.745973 flask_leaflet-0.1.2/flask_leaflet/templates/factory.html
+-rwxr-xr-x   0        0        0      981 2023-05-18 06:39:27.827607 flask_leaflet-0.1.2/flask_leaflet/templates/load.html
+-rwxr-xr-x   0        0        0      517 2023-05-18 06:46:02.709535 flask_leaflet-0.1.2/flask_leaflet/templates/map.html
+-rwxr-xr-x   0        0        0      366 2023-05-18 06:46:54.377132 flask_leaflet-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4705 1970-01-01 00:00:00.000000 flask_leaflet-0.1.2/PKG-INFO
```

### Comparing `flask_leaflet-0.1.1/README.md` & `flask_leaflet-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/__init__.py` & `flask_leaflet-0.1.2/flask_leaflet/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/basic_types.py` & `flask_leaflet-0.1.2/flask_leaflet/basic_types.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/layers/base.py` & `flask_leaflet-0.1.2/flask_leaflet/layers/base.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/layers/paths.py` & `flask_leaflet-0.1.2/flask_leaflet/layers/paths.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/layers/raster.py` & `flask_leaflet-0.1.2/flask_leaflet/layers/raster.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/layers/ui.py` & `flask_leaflet-0.1.2/flask_leaflet/layers/ui.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/map.py` & `flask_leaflet-0.1.2/flask_leaflet/map.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/mixins.py` & `flask_leaflet-0.1.2/flask_leaflet/mixins.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/static/images/marker-icon.png` & `flask_leaflet-0.1.2/flask_leaflet/static/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/static/images/marker-shadow.png` & `flask_leaflet-0.1.2/flask_leaflet/static/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/templates/dict_as_json.jinja` & `flask_leaflet-0.1.2/flask_leaflet/templates/dict_as_json.jinja`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/templates/factory.html` & `flask_leaflet-0.1.2/flask_leaflet/templates/factory.html`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/templates/load.html` & `flask_leaflet-0.1.2/flask_leaflet/templates/load.html`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.1/flask_leaflet/templates/map.html` & `flask_leaflet-0.1.2/flask_leaflet/templates/map.html`

 * *Files 4% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 })
 
 {% for layer in map._layers %}
     {{ layer() }}
     {{ layer.var_name }}.{{ layer.__bind_str__ }}( {{ map.var_name }} );
 {% endfor %}
 
-{% if not map.has_any_raster_layer() and leafletjs.default_tile_layer is not none %}
-    {{ leafletjs.default_tile_layer(map=map) }}
+{% if not map.has_any_raster_layer() and leaflet.default_tile_layer is not none %}
+    {{ leaflet.default_tile_layer(map=map) }}
 {% endif %}
 
 </script>
```

### Comparing `flask_leaflet-0.1.1/PKG-INFO` & `flask_leaflet-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-leaflet
-Version: 0.1.1
+Version: 0.1.2
 Author-Email: Sebastian Salinas <seba.salinas.delrio@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: flask>=2.3.2
 Description-Content-Type: text/markdown
 
 # Flask-Leaflet
```

