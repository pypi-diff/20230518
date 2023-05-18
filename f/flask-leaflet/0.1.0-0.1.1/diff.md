# Comparing `tmp/flask_leaflet-0.1.0.tar.gz` & `tmp/flask_leaflet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_leaflet-0.1.0.tar", last modified: Thu May 18 06:31:07 2023, max compression
+gzip compressed data, was "flask_leaflet-0.1.1.tar", last modified: Thu May 18 06:41:10 2023, max compression
```

## Comparing `flask_leaflet-0.1.0.tar` & `flask_leaflet-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     4478 2023-05-18 06:24:55.459001 flask_leaflet-0.1.0/README.md
--rwxr-xr-x   0        0        0     2681 2023-05-18 06:17:57.839724 flask_leaflet-0.1.0/flask_leaflet/__init__.py
--rwxr-xr-x   0        0        0     1593 2023-05-14 08:31:30.463333 flask_leaflet-0.1.0/flask_leaflet/basic_types.py
--rwxr-xr-x   0        0        0        0 2023-05-11 15:07:50.000000 flask_leaflet-0.1.0/flask_leaflet/layers/__init__.py
--rwxr-xr-x   0        0        0     1018 2023-05-18 04:18:13.595361 flask_leaflet-0.1.0/flask_leaflet/layers/base.py
--rwxr-xr-x   0        0        0     5030 2023-05-18 04:33:07.698015 flask_leaflet-0.1.0/flask_leaflet/layers/paths.py
--rwxr-xr-x   0        0        0     9359 2023-05-15 05:42:11.854584 flask_leaflet-0.1.0/flask_leaflet/layers/raster.py
--rwxr-xr-x   0        0        0     8981 2023-05-15 06:37:46.212225 flask_leaflet-0.1.0/flask_leaflet/layers/ui.py
--rwxr-xr-x   0        0        0     2551 2023-05-18 06:27:35.626652 flask_leaflet-0.1.0/flask_leaflet/map.py
--rwxr-xr-x   0        0        0     2169 2023-05-15 06:17:34.702685 flask_leaflet-0.1.0/flask_leaflet/mixins.py
--rwxr-xr-x   0        0        0     1466 2023-05-14 03:46:14.846425 flask_leaflet-0.1.0/flask_leaflet/static/images/marker-icon.png
--rwxr-xr-x   0        0        0      618 2023-05-14 03:46:19.848035 flask_leaflet-0.1.0/flask_leaflet/static/images/marker-shadow.png
--rwxr-xr-x   0        0        0     1321 2023-05-14 07:53:24.704663 flask_leaflet-0.1.0/flask_leaflet/templates/dict_as_json.jinja
--rwxr-xr-x   0        0        0      518 2023-05-15 06:24:24.745973 flask_leaflet-0.1.0/flask_leaflet/templates/factory.html
--rwxr-xr-x   0        0        0      989 2023-05-14 07:12:47.494751 flask_leaflet-0.1.0/flask_leaflet/templates/load.html
--rwxr-xr-x   0        0        0      521 2023-05-15 06:24:44.124066 flask_leaflet-0.1.0/flask_leaflet/templates/map.html
--rwxr-xr-x   0        0        0      366 2023-05-18 06:31:07.530343 flask_leaflet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4705 1970-01-01 00:00:00.000000 flask_leaflet-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     4478 2023-05-18 06:24:55.459001 flask_leaflet-0.1.1/README.md
+-rwxr-xr-x   0        0        0     2677 2023-05-18 06:39:38.258949 flask_leaflet-0.1.1/flask_leaflet/__init__.py
+-rwxr-xr-x   0        0        0     1593 2023-05-14 08:31:30.463333 flask_leaflet-0.1.1/flask_leaflet/basic_types.py
+-rwxr-xr-x   0        0        0        0 2023-05-11 15:07:50.000000 flask_leaflet-0.1.1/flask_leaflet/layers/__init__.py
+-rwxr-xr-x   0        0        0     1018 2023-05-18 04:18:13.595361 flask_leaflet-0.1.1/flask_leaflet/layers/base.py
+-rwxr-xr-x   0        0        0     5030 2023-05-18 04:33:07.698015 flask_leaflet-0.1.1/flask_leaflet/layers/paths.py
+-rwxr-xr-x   0        0        0     9359 2023-05-15 05:42:11.854584 flask_leaflet-0.1.1/flask_leaflet/layers/raster.py
+-rwxr-xr-x   0        0        0     8981 2023-05-15 06:37:46.212225 flask_leaflet-0.1.1/flask_leaflet/layers/ui.py
+-rwxr-xr-x   0        0        0     2551 2023-05-18 06:27:35.626652 flask_leaflet-0.1.1/flask_leaflet/map.py
+-rwxr-xr-x   0        0        0     2169 2023-05-15 06:17:34.702685 flask_leaflet-0.1.1/flask_leaflet/mixins.py
+-rwxr-xr-x   0        0        0     1466 2023-05-14 03:46:14.846425 flask_leaflet-0.1.1/flask_leaflet/static/images/marker-icon.png
+-rwxr-xr-x   0        0        0      618 2023-05-14 03:46:19.848035 flask_leaflet-0.1.1/flask_leaflet/static/images/marker-shadow.png
+-rwxr-xr-x   0        0        0     1321 2023-05-14 07:53:24.704663 flask_leaflet-0.1.1/flask_leaflet/templates/dict_as_json.jinja
+-rwxr-xr-x   0        0        0      518 2023-05-15 06:24:24.745973 flask_leaflet-0.1.1/flask_leaflet/templates/factory.html
+-rwxr-xr-x   0        0        0      981 2023-05-18 06:39:27.827607 flask_leaflet-0.1.1/flask_leaflet/templates/load.html
+-rwxr-xr-x   0        0        0      521 2023-05-15 06:24:44.124066 flask_leaflet-0.1.1/flask_leaflet/templates/map.html
+-rwxr-xr-x   0        0        0      366 2023-05-18 06:41:10.088427 flask_leaflet-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4705 1970-01-01 00:00:00.000000 flask_leaflet-0.1.1/PKG-INFO
```

### Comparing `flask_leaflet-0.1.0/README.md` & `flask_leaflet-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/__init__.py` & `flask_leaflet-0.1.1/flask_leaflet/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
     def __init__(self, app: Optional[Flask] = None) -> None:
         if app is not None:
             self.init_app(app)
 
     def __register_blueprint(self, app: Flask) -> Blueprint:
         blueprint = Blueprint(
-            "leafletjs",
+            "leaflet",
             __name__,
             template_folder="templates",
             static_folder="static",
-            static_url_path="/leafletjs/static",
+            static_url_path="/leaflet/static",
         )
         app.register_blueprint(blueprint)
 
     def init_app(self, app: Flask) -> None:
         if not hasattr(app, "extensions"):
             app.extensions = {}
         app.extensions["leaflet"] = self
```

### Comparing `flask_leaflet-0.1.0/flask_leaflet/basic_types.py` & `flask_leaflet-0.1.1/flask_leaflet/basic_types.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/layers/base.py` & `flask_leaflet-0.1.1/flask_leaflet/layers/base.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/layers/paths.py` & `flask_leaflet-0.1.1/flask_leaflet/layers/paths.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/layers/raster.py` & `flask_leaflet-0.1.1/flask_leaflet/layers/raster.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/layers/ui.py` & `flask_leaflet-0.1.1/flask_leaflet/layers/ui.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/map.py` & `flask_leaflet-0.1.1/flask_leaflet/map.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/mixins.py` & `flask_leaflet-0.1.1/flask_leaflet/mixins.py`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/static/images/marker-icon.png` & `flask_leaflet-0.1.1/flask_leaflet/static/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/static/images/marker-shadow.png` & `flask_leaflet-0.1.1/flask_leaflet/static/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/templates/dict_as_json.jinja` & `flask_leaflet-0.1.1/flask_leaflet/templates/dict_as_json.jinja`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/templates/factory.html` & `flask_leaflet-0.1.1/flask_leaflet/templates/factory.html`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/flask_leaflet/templates/load.html` & `flask_leaflet-0.1.1/flask_leaflet/templates/load.html`

 * *Files 13% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 {% else %}
 <script nonce={{ csp_nonce() if csp_nonce else "" }} src="https://unpkg.com/leaflet@{{ js_version }}/dist/leaflet.js"
      integrity="sha256-WBkoXOwTeyKclOHuWtc+i2uENFpDZ9YPdf5Hf+D7ewM="
      crossorigin=""></script>
 {% endif %}
 <script nonce={{ csp_nonce() if csp_nonce else "" }} >
      var leaflet_default_icon = L.icon({
-          iconUrl: "{{ leafletjs.default_icon_marker_url or url_for('leafletjs.static', filename='images/marker-icon.png') }}",
-          shadowUrl: "{{ leafletjs.default_icon_marker_shadow_url or url_for('leafletjs.static', filename='images/marker-shadow.png') }}",
+          iconUrl: "{{ leaflet.default_icon_marker_url or url_for('leaflet.static', filename='images/marker-icon.png') }}",
+          shadowUrl: "{{ leaflet.default_icon_marker_shadow_url or url_for('leaflet.static', filename='images/marker-shadow.png') }}",
           iconAnchor: [12.5,41],
      }) 
 </script>
```

#### html2text {}

```diff
@@ -3,11 +3,11 @@
  {% endif %} {% if js_local_path %}
  {% else %}
 ) if csp_nonce else "" }} src="https://unpkg.com/leaflet@{{ js_version }}/dist/
 leaflet.js" integrity="sha256-WBkoXOwTeyKclOHuWtc+i2uENFpDZ9YPdf5Hf+D7ewM="
 crossorigin="">
 {% endif %}
 ) if csp_nonce else "" }} > var leaflet_default_icon = L.icon({ iconUrl: "{
-{ leafletjs.default_icon_marker_url or url_for('leafletjs.static',
+{ leaflet.default_icon_marker_url or url_for('leaflet.static',
 filename='images/marker-icon.png') }}", shadowUrl: "{
-{ leafletjs.default_icon_marker_shadow_url or url_for('leafletjs.static',
+{ leaflet.default_icon_marker_shadow_url or url_for('leaflet.static',
 filename='images/marker-shadow.png') }}", iconAnchor: [12.5,41], })
```

### Comparing `flask_leaflet-0.1.0/flask_leaflet/templates/map.html` & `flask_leaflet-0.1.1/flask_leaflet/templates/map.html`

 * *Files identical despite different names*

### Comparing `flask_leaflet-0.1.0/PKG-INFO` & `flask_leaflet-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-leaflet
-Version: 0.1.0
+Version: 0.1.1
 Author-Email: Sebastian Salinas <seba.salinas.delrio@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: flask>=2.3.2
 Description-Content-Type: text/markdown
 
 # Flask-Leaflet
```

